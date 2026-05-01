---
description: Returns details of a resource evaluation based on the selected filter.
layout: schema
name: ResourceEvaluationFilters
properties_list:
- description: ''
  name: EvaluationMode
  type: object
- description: ''
  name: TimeWindow
  type: object
- description: ''
  name: EvaluationContextIdentifier
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-resource-evaluation-filters-schema.json
slug: config-resource-evaluation-filters
source_filename: config-resource-evaluation-filters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-evaluation-filters-schema.json\",\n  \"title\": \"ResourceEvaluationFilters\",\n  \"description\": \"Returns details of a resource evaluation based on the selected filter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EvaluationMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationMode\"\n        },\n        {\n          \"description\": \"Filters all resource evaluations results based on an evaluation mode. the valid value for this API is <code>Proactive</code>.\"\n        }\n      ]\n    },\n    \"TimeWindow\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeWindow\"\n        },\n        {\n          \"description\": \"Returns a <code>TimeWindow</code> object.\"\n        }\n      ]\n    },\n    \"EvaluationContextIdentifier\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationContextIdentifier\"\n        },\n        {\n          \"description\": \"Filters evaluations for a given infrastructure deployment. For example: CFN Stack.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-evaluation-filters-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: ResourceEvaluationFilters
---
