---
description: ApplicationHostResponseType schema
layout: schema
name: ApplicationHostResponseType
properties_list:
- description: ''
  name: host
  type: string
- description: ''
  name: application_name
  type: string
- description: ''
  name: application_summary
  type: object
- description: ''
  name: end_user_summary
  type: object
- description: ''
  name: health_status
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: language
  type: integer
- description: ''
  name: links
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-application-host-response-type-schema.json
slug: openapi-application-host-response-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-application-host-response-type-schema.json\",\n  \"title\": \"ApplicationHostResponseType\",\n  \"description\": \"ApplicationHostResponseType schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"host\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"application_name\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"application_summary\": {\n      \"$ref\": \"#/components/schemas/AppSummaryDataResponse\"\n    },\n    \"end_user_summary\": {\n      \"$ref\": \"#/components/schemas/EndUserSummaryDataResponse\"\n    },\n    \"health_status\": {\n      \"type\": \"string\",\n      \"example\": \"active\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"language\": {\n      \"type\"\
  : \"integer\",\n      \"example\": 100\n    },\n    \"links\": {\n      \"$ref\": \"#/components/schemas/ApplicationHostLinksResponse\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-application-host-response-type-schema.json
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
title: ApplicationHostResponseType
---
