# ADR-001 — Adotar modelo híbrido

**Status:** Aceita conceitualmente

## Contexto
Uma empresa deve representar o que sabe, faz, decide, aprende e modifica. Apenas pastas/documentos ou apenas busca vetorial não garantem contexto, temporalidade e autoridade.

## Decisão
Usar entidades relacionais tipadas, processos versionados, afirmações contextualizadas, evidências preservadas, grafo de relacionamentos e governança de autoridade/validade. PostgreSQL como núcleo inicial.

## Consequências
+ Integridade e rastreabilidade.
+ Recuperação contextual por agentes.
+ Evolução modular e extensão setorial.
- Maior esforço de modelagem.
- Necessidade de políticas de publicação e resolução de conflitos.

## Alternativas não adotadas como núcleo exclusivo
Pastas documentais; RAG vetorial isolado; banco de grafos isolado; modelo EAV sem tipos.
