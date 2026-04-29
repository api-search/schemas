---
description: ListSpacesRequest schema from Amazon CodeCatalyst
layout: schema
name: ListSpacesRequest
properties_list:
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-list-spaces-request-schema.json
slug: amazon-codecatalyst-list-spaces-request
source_filename: amazon-codecatalyst-list-spaces-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-list-spaces-request-schema.json\",\n  \"title\": \"ListSpacesRequest\",\n  \"description\": \"ListSpacesRequest schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListSpacesRequestNextTokenString\"\n        },\n        {\n          \"description\": \"A token returned from a call to this API to indicate the next batch of results to return, if any.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-list-spaces-request-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: ListSpacesRequest
---
