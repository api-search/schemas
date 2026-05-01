---
description: Response from the CreateRule action
layout: schema
name: CreateRuleResponse
properties_list:
- description: Information about the rule
  name: rules
  type: array
provider_name: Amazon Elastic Load Balancing
provider_slug: amazon-elastic-load-balancing
schema_file: json-schema/amazon-elastic-load-balancing-create-rule-response-schema.json
slug: amazon-elastic-load-balancing-create-rule-response
source_filename: amazon-elastic-load-balancing-create-rule-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-create-rule-response-schema.json\",\n  \"title\": \"CreateRuleResponse\",\n  \"description\": \"Response from the CreateRule action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rules\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the rule\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Rule\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-create-rule-response-schema.json
tags:
- Amazon Web Services
- High Availability
- Load Balancing
- Networking
- Scalability
title: CreateRuleResponse
---
