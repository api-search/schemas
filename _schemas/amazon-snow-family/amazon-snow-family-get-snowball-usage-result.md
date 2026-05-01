---
description: GetSnowballUsageResult schema from Amazon Snow Family API
layout: schema
name: GetSnowballUsageResult
properties_list:
- description: ''
  name: SnowballLimit
  type: object
- description: ''
  name: SnowballsInUse
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-get-snowball-usage-result-schema.json
slug: amazon-snow-family-get-snowball-usage-result
source_filename: amazon-snow-family-get-snowball-usage-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-get-snowball-usage-result-schema.json\",\n  \"title\": \"GetSnowballUsageResult\",\n  \"description\": \"GetSnowballUsageResult schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnowballLimit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The service limit for number of Snow devices this account can have at once. The default service limit is 1 (one).\"\n        }\n      ]\n    },\n    \"SnowballsInUse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of Snow devices that this account is currently using.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-get-snowball-usage-result-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: GetSnowballUsageResult
---
