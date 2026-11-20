# Arquitetura do Conhecimento — SCCO

Sistema de Conhecimento e Consciência Organizacional. Projeto conceitual e técnico para representar o que uma empresa sabe, faz, decide, aprende e modifica, com contexto, autoridade, temporalidade e proveniência.

## Estado
Documentação de referência inicial, consolidada a partir das discussões conceituais. **Não é software implementado nem esquema de produção validado.**

## Decisão central
Modelo híbrido: entidades tipadas + processos e execuções + afirmações contextualizadas + evidências multimodais + grafo de relacionamentos + governança temporal.

## Leitura sugerida
1. `docs/01-visao-estrategica.md`
2. `docs/02-principios-arquiteturais.md`
3. `docs/03-ontologia-empresarial.md`
4. `docs/04-entidades-e-relacionamentos.md`
5. `docs/05-modelo-de-conhecimento.md`
6. `docs/06-governanca-e-autoridade.md`
7. `docs/07-processos-e-eventos.md`
8. `docs/08-agentes-de-ia.md`
9. `docs/09-roadmap.md`
10. `database/schema-inicial.sql`

## Próximo trabalho
Detalhar núcleo universal e escrever migrações testadas: tenancy, temporalidade bitemporal, claims tipados, autoridade, workflow, proveniência, políticas de acesso e testes de conflitos.

## Estrutura do repositório

| Pasta | Finalidade |
| --- | --- |
| [docs/](docs/README.md) | Visão, princípios, modelo, governança e roadmap |
| [decisions/](decisions/README.md) | Registro das decisões arquiteturais |
| [ontology/](ontology/README.md) | Formalização futura da ontologia universal |
| [database/](database/README.md) | Esquema exploratório e migrações futuras |
| [src/](src/README.md) | Implementação futura do produto |

## Como contribuir

Leia [AGENTS.md](AGENTS.md) e o [ADR-001](decisions/ADR-001-modelo-hibrido.md). Trabalhe em incrementos rastreáveis, preserve fontes e histórico e registre decisões novas em ADRs. Não inclua credenciais ou documentos empresariais confidenciais no Git.

Ainda não há comandos de instalação, execução ou testes: o projeto está na etapa de modelagem. Consulte o [roadmap](docs/09-roadmap.md) para os marcos e critérios de aceitação e o [registro de inicialização](docs/inicializacao.md) para o inventário preservado.
