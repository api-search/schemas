---
description: Response containing a paginated list of incidents
layout: schema
name: IncidentsResponse
properties_list:
- description: List of incident objects
  name: data
  type: array
- description: Related resources included in the response based on the include query parameter
  name: included
  type: array
- description: Metadata about the incidents list response
  name: meta
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-incidents-incidents-response-schema.json
slug: datadog-incidents-incidents-response
source_filename: datadog-incidents-incidents-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incidents-response-schema.json\",\n  \"title\": \"IncidentsResponse\",\n  \"description\": \"Response containing a paginated list of incidents\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"List of incident objects\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Incident\"\n      }\n    },\n    \"included\": {\n      \"type\": \"array\",\n      \"description\": \"Related resources included in the response based on the include query parameter\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about the incidents list response\",\n      \"properties\": {\n        \"pagination\": {\n          \"type\": \"object\"\
  ,\n          \"description\": \"Pagination information for navigating through results\",\n          \"properties\": {\n            \"next_offset\": {\n              \"type\": \"integer\",\n              \"description\": \"The offset to use in the next request to retrieve the next page\"\n            },\n            \"prev_offset\": {\n              \"type\": \"integer\",\n              \"description\": \"The offset to use to retrieve the previous page\"\n            },\n            \"size\": {\n              \"type\": \"integer\",\n              \"description\": \"The number of incidents in this page\"\n            },\n            \"total_count\": {\n              \"type\": \"integer\",\n              \"description\": \"The total number of incidents matching the filter criteria\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-incidents-incidents-response-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: IncidentsResponse
---
