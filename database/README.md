# Banco de dados

[Esquema inicial](schema-inicial.sql) é um estudo exploratório PostgreSQL preservado sem alterações. Não executar em produção.

`migrations/` fica reservado a migrações versionadas e testadas. O esquema inicial não é uma migração de produção.

Antes da implementação: completar isolamento por tenant e chaves compostas, autorização/RLS, histórico bitemporal, aprovação, predicados tipados e tratamento de conflitos. Referências: [princípios](../docs/02-principios-arquiteturais.md) e [ADR-001](../decisions/ADR-001-modelo-hibrido.md).
