---
description: Entity Match object showing the decision reached for each Entity.
layout: schema
name: EntityMatch
properties_list:
- description: FactSet Entity Identifier of the entity matched respective to the requested Name submitted. For more detail, visit [FactSet Permanent Security Identifier](https://oa.apps.factset.com/cms/oaAttachment/
  name: entityId
  type: string
- description: Full name corresponding to the matched entity.
  name: entityName
  type: string
- description: ISO2 country code corresponding to the location of the matched entity.
  name: countryCode
  type: string
- description: Code representing the entity type of the matched entity. See the related request parameter for a table of all Codes and their respective descriptions.
  name: entityTypeCode
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-private-markets-entity-match-schema.json
slug: factset-private-markets-entity-match
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EntityMatch\",\n  \"type\": \"object\",\n  \"description\": \"Entity Match object showing the decision reached for each Entity.\\n\",\n  \"properties\": {\n    \"entityId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Entity Identifier of the entity matched respective to the requested Name submitted. For more detail, visit [FactSet Permanent Security Identifier](https://oa.apps.factset.com/cms/oaAttachment/64c3213a-f415-4c27-a336-92c73a72deed/24881)\\n\"\n    },\n    \"entityName\": {\n      \"type\": \"string\",\n      \"description\": \"Full name corresponding to the matched entity.\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO2 country code corresponding to the location of the matched entity.\"\n    },\n    \"entityTypeCode\": {\n      \"type\": \"string\",\n      \"description\": \"Code representing the entity type of the\
  \ matched entity. See the related request parameter for a table of all Codes and their respective descriptions.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-private-markets-entity-match-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: EntityMatch
---
