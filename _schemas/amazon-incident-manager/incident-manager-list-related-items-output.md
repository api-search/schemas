---
description: ListRelatedItemsOutput schema
layout: schema
name: ListRelatedItemsOutput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: relatedItems
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-list-related-items-output-schema.json
slug: incident-manager-list-related-items-output
source_filename: incident-manager-list-related-items-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-list-related-items-output-schema.json\",\n  \"title\": \"ListRelatedItemsOutput\",\n  \"description\": \"ListRelatedItemsOutput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token to continue to the next page of results.\"\n        }\n      ]\n    },\n    \"relatedItems\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelatedItemList\"\n        },\n        {\n          \"description\": \"Details about each related item.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"relatedItems\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-list-related-items-output-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: ListRelatedItemsOutput
---
