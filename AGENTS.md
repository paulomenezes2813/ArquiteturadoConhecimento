# Instruções para agentes de desenvolvimento — SCCO

## Missão
Desenvolver uma plataforma de conhecimento empresarial confiável, multimodal, auditável, contextual, temporal e reutilizável por agentes de IA.

## Decisões já tomadas
- Arquitetura híbrida, não apenas RAG ou banco vetorial.
- Separar entidade, afirmação, evidência e conhecimento institucional.
- Identidade permanente separada de versões.
- Preservar fontes originais e histórico; não sobrescrever silenciosamente.
- Toda afirmação tem escopo, origem, vigência e status.
- IA pode propor, não oficializar autonomamente normas.
- Resolver regras por contexto, autoridade, vigência e permissões.
- PostgreSQL como banco transacional inicial; grafo por arestas tipadas no PostgreSQL, sem exigir banco de grafos dedicado no MVP.
- Conteúdo multimodal em armazenamento de objetos, com segmentos referenciáveis.
- Separar definição de processo de instância executada.
- APIs para consulta, resolução, proveniência, dependências, propostas, conflitos e histórico.

## Guardrails de implementação
- Nunca afirmar que uma hipótese ou extração foi aprovada sem workflow.
- Isolar dados por organização/tenant inclusive em chaves estrangeiras e autorização.
- Exigir autenticação e aplicar autorização no servidor antes de recuperar conteúdo.
- Não confiar em papel declarado pelo cliente ou prompt.
- Não assumir que dado mais recente tem maior autoridade.
- Não apagar evidências para eliminar redundância; consolidar a referência canônica.
- Não criar tabelas setoriais prematuramente.
- Não apresentar `schema-inicial.sql` como pronto para produção.
- Propor alterações arquiteturais como ADRs, explicitando trade-offs.
- Incluir testes para conflitos, escopo, versões, autorização e proveniência.

## Fluxo de trabalho
1. Ler README e documentação de domínio.
2. Escrever proposta e testes de aceitação.
3. Implementar incrementalmente, sem quebrar decisões registradas.
4. Documentar migrações, decisões e riscos.
5. Não inventar regras de negócio ausentes; registrar pendências.

## Organização do repositório
- `docs/`: especificações e referências conceituais existentes.
- `decisions/`: ADRs numerados; preservar decisões anteriores e explicitar substituições.
- `ontology/`: definições formais futuras, referenciando os documentos de domínio.
- `database/`: esquema exploratório; `migrations/` para migrações futuras verificadas.
- `src/`: código futuro; não presumir linguagem ou framework já aprovado.

## Verificação e entrega
- Conferir `git status` e alterações locais antes de editar.
- Preservar documentos de referência; registrar motivo e proveniência das revisões.
- Em mudanças documentais, verificar links e consistência com o ADR e o domínio.
- Em implementação, executar os testes pertinentes e informar comandos e resultados; não declarar testes inexistentes como aprovados.
- Nunca versionar segredos, arquivos `.env` ou dados empresariais privados.
- Não apresentar a estrutura de pastas como implementação concluída.
