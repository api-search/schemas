---
description: DescribeAttackResponse schema from api
layout: schema
name: DescribeAttackResponse
properties_list:
- description: ''
  name: Attack
  type: object
provider_name: Amazon Shield
provider_slug: amazon-shield
schema_file: json-schema/amazon-shield-api-describe-attack-response-schema.json
slug: amazon-shield-api-describe-attack-response
source_filename: amazon-shield-api-describe-attack-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/json-schema/amazon-shield-api-describe-attack-response-schema.json\",\n  \"title\": \"DescribeAttackResponse\",\n  \"description\": \"DescribeAttackResponse schema from api\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Attack\": {\n      \"$ref\": \"#/components/schemas/AttackDetail\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/json-schema/amazon-shield-api-describe-attack-response-schema.json
tags:
- DDoS Protection
- Networking
- Security
title: DescribeAttackResponse
---
