# Registro de inicialização — 20 de novembro de 2026

## Estado encontrado antes das alterações

A pasta do chat estava vazia, contendo apenas `work/` e `outputs/`, sem Git. A Page do projeto apontava para `/Users/paulomenezes/git/Arquitetura do Conhecimento`.

Nessa pasta havia um pacote ZIP e uma pasta extraída `ArquiteturadoConhecimento`, também sem `.git`. A pasta extraída foi adotada como raiz do projeto. Não havia branch, commits ou remoto a preservar.

## Inventário preservado

- Nove documentos numerados de `docs/01-visao-estrategica.md` a `docs/09-roadmap.md`, sem alterações.
- `decisions/ADR-001-modelo-hibrido.md`, sem alterações.
- `database/schema-inicial.sql`, sem alterações.
- README e AGENTS existentes, ampliados sem remover seu conteúdo original.
- ZIP original mantido fora da raiz do projeto.

## Organização

Adicionados índices, diretórios de ontologia e código, espaço para migrações e regras para ignorar arquivos locais e segredos. Nenhuma nova decisão técnica substitui o ADR-001. PostgreSQL, arquitetura híbrida, fontes preservadas, identidade/versionamento separados, governança humana e segregação por organização continuam como referências.

## Limites e próximos passos

Não há aplicação, dependências, testes automatizados ou migrações validadas. A verificação desta etapa cobre preservação dos documentos, estrutura e links locais; não valida o SQL como solução de produção. Seguir o roadmap existente para detalhar o núcleo universal e os critérios de aceitação antes de implementar.
