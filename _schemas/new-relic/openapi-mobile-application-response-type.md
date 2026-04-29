---
description: MobileApplicationResponseType schema
layout: schema
name: MobileApplicationResponseType
properties_list:
- description: ''
  name: crash_summary
  type: object
- description: ''
  name: health_status
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: mobile_summary
  type: object
- description: ''
  name: name
  type: string
- description: ''
  name: reporting
  type: boolean
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-mobile-application-response-type-schema.json
slug: openapi-mobile-application-response-type
source_filename: openapi-mobile-application-response-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-mobile-application-response-type-schema.json\",\n  \"title\": \"MobileApplicationResponseType\",\n  \"description\": \"MobileApplicationResponseType schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"crash_summary\": {\n      \"$ref\": \"#/components/schemas/CrashSummaryResponse\"\n    },\n    \"health_status\": {\n      \"type\": \"string\",\n      \"example\": \"active\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"mobile_summary\": {\n      \"$ref\": \"#/components/schemas/MobileSummaryDataResponse\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-resource-01\"\n    },\n    \"reporting\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-mobile-application-response-type-schema.json
tags:
- Analysis
- Analytics
- APM
- DevOps
- Infrastructure
- Monitoring
- Observability
- Performance
- Platform
title: MobileApplicationResponseType
---
