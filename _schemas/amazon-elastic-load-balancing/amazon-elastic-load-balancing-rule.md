---
description: Describes a rule
layout: schema
name: Rule
properties_list:
- description: The Amazon Resource Name (ARN) of the rule
  name: ruleArn
  type: string
- description: The priority of the rule
  name: priority
  type: string
- description: The conditions for the rule
  name: conditions
  type: array
- description: The actions for the rule
  name: actions
  type: array
- description: Whether this is the default rule
  name: isDefault
  type: boolean
provider_name: Amazon Elastic Load Balancing
provider_slug: amazon-elastic-load-balancing
schema_file: json-schema/amazon-elastic-load-balancing-rule-schema.json
slug: amazon-elastic-load-balancing-rule
source_filename: amazon-elastic-load-balancing-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-rule-schema.json\",\n  \"title\": \"Rule\",\n  \"description\": \"Describes a rule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ruleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the rule\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"The priority of the rule\"\n    },\n    \"conditions\": {\n      \"type\": \"array\",\n      \"description\": \"The conditions for the rule\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"field\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the field\"\n          },\n          \"values\": {\n            \"type\": \"array\",\n            \"description\"\
  : \"The condition values\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"actions\": {\n      \"type\": \"array\",\n      \"description\": \"The actions for the rule\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Action\"\n      }\n    },\n    \"isDefault\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the default rule\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-rule-schema.json
tags:
- Amazon Web Services
- High Availability
- Load Balancing
- Networking
- Scalability
title: Rule
---
