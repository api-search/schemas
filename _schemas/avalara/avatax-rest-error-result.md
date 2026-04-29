---
description: ErrorResult schema from Avalara API
layout: schema
name: ErrorResult
properties_list:
- description: ''
  name: error
  type: object
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-rest-error-result-schema.json
slug: avatax-rest-error-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-error-result-schema.json\",\n  \"title\": \"ErrorResult\",\n  \"description\": \"ErrorResult schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Machine-readable error code\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable error message\"\n        },\n        \"target\": {\n          \"type\": \"string\",\n          \"description\": \"The component that generated the error\"\n        },\n        \"details\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"code\": {\n \
  \               \"type\": \"string\"\n              },\n              \"number\": {\n                \"type\": \"integer\"\n              },\n              \"message\": {\n                \"type\": \"string\"\n              },\n              \"description\": {\n                \"type\": \"string\"\n              },\n              \"faultCode\": {\n                \"type\": \"string\"\n              },\n              \"helpLink\": {\n                \"type\": \"string\"\n              },\n              \"severity\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"Error\",\n                  \"Warning\",\n                  \"Exception\"\n                ]\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-rest-error-result-schema.json
tags:
- Taxes
title: ErrorResult
---
