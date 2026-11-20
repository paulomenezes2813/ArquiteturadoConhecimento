# Entidades e relacionamentos

## Distinções
- Entidade: objeto com identidade, ex. hotel.
- Afirmação: proposição sobre objeto, ex. capacidade de apartamentos.
- Evidência: fonte que sustenta ou contradiz afirmação.
- Conhecimento institucional: afirmação validada, vigente e autorizada.

## Vocabulário inicial de relações
`PART_OF`, `MEMBER_OF`, `PERFORMS`, `RESPONSIBLE_FOR`, `APPROVES`, `GOVERNS`, `IMPLEMENTS`, `DEPENDS_ON`, `USES`, `PRODUCES`, `MEASURED_BY`, `SUPPORTED_BY`, `CONTRADICTS`, `SUPERSEDES`, `DERIVED_FROM`, `APPLIES_TO`, `EXCEPTS`, `CHANGES`, `TRIGGERED_BY`, `AFFECTS`, `LEARNED_FROM`, `EXECUTED_BY`.

## Regras de modelagem
- Cada relação tem tipo, origem, destino, contexto e validade quando pertinente.
- Predicados definem tipos permitidos, cardinalidade e semântica de comparação.
- Não inferir contradição de valores diferentes sem comparar sujeito, predicado, escopo, tempo e exceções.
- Identificadores globais não dispensam integridade de tenant.
- Definição de processo e instância operacional são entidades diferentes.

## Exemplo
Decisão CHANGES Regra; Regra GOVERNS Processo; Processo USES Ativo; Ocorrência AFFECTS Processo; Lição LEARNED_FROM Ocorrência.
