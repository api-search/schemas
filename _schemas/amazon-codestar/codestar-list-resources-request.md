---
description: ListResourcesRequest schema from AWS CodeStar API
layout: schema
name: ListResourcesRequest
properties_list:
- description: ''
  name: projectId
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-list-resources-request-schema.json
slug: codestar-list-resources-request
source_filename: codestar-list-resources-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-list-resources-request-schema.json\",\n  \"title\": \"ListResourcesRequest\",\n  \"description\": \"ListResourcesRequest schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"projectId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectId\"\n        },\n        {\n          \"description\": \"The ID of the project.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The continuation token for the next set of results, if the results cannot be returned in one response.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\
  \n        },\n        {\n          \"description\": \"The maximum amount of data that can be contained in a single set of results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"projectId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-list-resources-request-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: ListResourcesRequest
---
