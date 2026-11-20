# Agentes de IA e API do conhecimento

## Operações previstas
- `knowledge.search`: localizar candidatos.
- `knowledge.get`: recuperar objeto/versão.
- `knowledge.resolve`: resolver conhecimento aplicável.
- `knowledge.trace`: mostrar evidências.
- `knowledge.dependencies`: avaliar impacto.
- `knowledge.propose`: propor alteração.
- `knowledge.conflicts`: consultar divergências.
- `knowledge.history`: consultar versões.

## Fluxo de resolução
1. Autenticar ator e identificar contexto.
2. Autorizar consulta no servidor.
3. Buscar candidatos por texto, semântica e grafo.
4. Filtrar escopo, vigência, precedência e exceções.
5. Detectar conflitos não resolvidos.
6. Responder com fonte e versão, ou indicar insuficiência.
7. Auditar acesso conforme criticidade.

## Segurança
O agente não pode se autoconceder permissões. Consulta não implica autorização para executar ação externa. Ações requerem ferramentas e políticas específicas.
