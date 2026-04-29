---
description: ListApplicationsResponse schema from AWS Mainframe Modernization API
layout: schema
name: ListApplicationsResponse
properties_list:
- description: ''
  name: applications
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-list-applications-response-schema.json
slug: amazon-mainframe-modernization-list-applications-response
source_filename: amazon-mainframe-modernization-list-applications-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-list-applications-response-schema.json\",\n  \"title\": \"ListApplicationsResponse\",\n  \"description\": \"ListApplicationsResponse schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applications\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationSummaryList\"\n        },\n        {\n          \"description\": \"Returns a list of summary details for all the applications in a runtime environment.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A pagination token that's returned when the response doesn't contain all applications.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applications\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-list-applications-response-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: ListApplicationsResponse
---
