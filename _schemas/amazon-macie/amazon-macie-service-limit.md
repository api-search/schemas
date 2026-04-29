---
description: Specifies a current quota for an Amazon Macie account.
layout: schema
name: ServiceLimit
properties_list:
- description: ''
  name: isServiceLimited
  type: object
- description: ''
  name: unit
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-service-limit-schema.json
slug: amazon-macie-service-limit
source_filename: amazon-macie-service-limit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-service-limit-schema.json\",\n  \"title\": \"ServiceLimit\",\n  \"description\": \"Specifies a current quota for an Amazon Macie account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"isServiceLimited\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the account has met the quota that corresponds to the metric specified by the UsageByAccount.type field in the response.\"\n        }\n      ]\n    },\n    \"unit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Unit\"\n        },\n        {\n          \"description\": \"The unit of measurement for the value specified by the value field.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The value for the metric specified by the UsageByAccount.type field in the response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-service-limit-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ServiceLimit
---
