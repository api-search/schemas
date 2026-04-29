---
description: ApplicationHostResponse schema
layout: schema
name: ApplicationHostResponse
properties_list:
- description: ''
  name: application_hosts
  type: array
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-application-host-response-schema.json
slug: openapi-application-host-response
source_filename: openapi-application-host-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-application-host-response-schema.json\",\n  \"title\": \"ApplicationHostResponse\",\n  \"description\": \"ApplicationHostResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application_hosts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ApplicationHostResponseType\"\n      },\n      \"example\": [\n        {\n          \"host\": \"example_string\",\n          \"application_name\": \"example_string\",\n          \"application_summary\": {},\n          \"end_user_summary\": {},\n          \"health_status\": \"active\",\n          \"id\": 100,\n          \"language\": 100,\n          \"links\": {}\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-application-host-response-schema.json
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
title: ApplicationHostResponse
---
