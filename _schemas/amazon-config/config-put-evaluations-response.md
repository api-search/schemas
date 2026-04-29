---
description: <p/>
layout: schema
name: PutEvaluationsResponse
properties_list:
- description: ''
  name: FailedEvaluations
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-evaluations-response-schema.json
slug: config-put-evaluations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-evaluations-response-schema.json\",\n  \"title\": \"PutEvaluationsResponse\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FailedEvaluations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Evaluations\"\n        },\n        {\n          \"description\": \"Requests that failed because of a client or server error.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-evaluations-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: PutEvaluationsResponse
---
