# Modelo de conhecimento

## Unidade de Conhecimento / OCE
Identificador permanente, tipo, nome, descrição, organização, domínio, contexto, proprietário, fonte, autoridade, classificação de acesso, vigência, versão, status e relações.

## Modelo de afirmações
Campos conceituais: `subject_id`, `predicate_id`, `object_id` ou `literal_value`, `scope_id`, `valid_from`, `valid_to`, `recorded_at`, `source_id`, `authority_id`, `status`, `knowledge_version_id`.

## Princípios
- Uma afirmação não é automaticamente verdade institucional.
- `confidence` de IA é confiança de extração, não autorização normativa.
- Preservar texto original, segmentos de fonte e links de proveniência.
- Não apagar documentos redundantes: centralizar a referência institucional e manter evidências.
- Suportar dados multivalorados, incerteza e exceções.

## Temporalidade
Distinguir tempo de validade (quando regra se aplica) e tempo de registro (quando sistema soube). Consultas históricas devem selecionar versões corretas.

## Conflito
Possível conflito: mesmo sujeito, predicado, contexto e período sobreposto com valores incompatíveis, após considerar precedência e cardinalidade.
