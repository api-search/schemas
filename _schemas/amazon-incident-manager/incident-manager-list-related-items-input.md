---
description: ListRelatedItemsInput schema
layout: schema
name: ListRelatedItemsInput
properties_list:
- description: ''
  name: incidentRecordArn
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-list-related-items-input-schema.json
slug: incident-manager-list-related-items-input
source_filename: incident-manager-list-related-items-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-list-related-items-input-schema.json\",\n  \"title\": \"ListRelatedItemsInput\",\n  \"description\": \"ListRelatedItemsInput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"incidentRecordArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the incident record containing the listed related items.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of related items per page.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\
  \n        },\n        {\n          \"description\": \"The pagination token to continue to the next page of results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"incidentRecordArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-list-related-items-input-schema.json
tags:
- Automation
- DevOps
- Incident Management
- Operations
title: ListRelatedItemsInput
---
