# Princípios arquiteturais

1. Identidade permanente para objetos relevantes.
2. Separar identidade de conteúdo versionado.
3. Toda afirmação institucional deve possuir origem rastreável.
4. Conhecimento possui contexto e vigência.
5. Preservar histórico de decisões e alterações.
6. Regras oficiais possuem autoridade responsável.
7. Conectar conhecimentos, processos, pessoas, ativos e evidências.
8. Detectar contradições sem presumir que diferenças são conflitos.
9. IA extrai e propõe; autoridade competente valida e publica.
10. Respostas respeitam permissão, escopo, temporalidade e precedência.
11. Separar dados transacionais vivos de conhecimento relativamente estável.
12. Mudanças relevantes geram análise de impacto.
13. Publicações críticas são transacionais e auditáveis.
14. Governança e privacidade são requisitos estruturais, não opcionais.

## Arquitetura técnica inicial
- PostgreSQL: entidades tipadas, relações, versões, governança.
- Armazenamento S3 compatível: arquivos originais.
- Busca textual e vetorial: recuperação de candidatos.
- Grafo por `graph_edges` inicialmente.
- Serviços: ingestão, extração, curadoria, resolução, aprovação, auditoria.
- APIs e ferramentas MCP para agentes, sob autenticação.

## Atenção
Semântica e autorização não podem depender somente da similaridade vetorial ou de confiança estatística do modelo.
