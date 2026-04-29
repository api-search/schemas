---
description: ListEnvironmentsResponse schema from AWS Mainframe Modernization API
layout: schema
name: ListEnvironmentsResponse
properties_list:
- description: ''
  name: environments
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-list-environments-response-schema.json
slug: amazon-mainframe-modernization-list-environments-response
source_filename: amazon-mainframe-modernization-list-environments-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-list-environments-response-schema.json\",\n  \"title\": \"ListEnvironmentsResponse\",\n  \"description\": \"ListEnvironmentsResponse schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"environments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentSummaryList\"\n        },\n        {\n          \"description\": \"Returns a list of summary details for all the runtime environments in your account. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A pagination token that's returned when the response doesn't contain all the runtime environments.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"environments\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-list-environments-response-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: ListEnvironmentsResponse
---
