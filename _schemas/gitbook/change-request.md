---
description: A change request in GitBook represents a proposed set of content changes to a space, similar to a pull request. Change requests support collaborative review workflows before merging into the main content.
layout: schema
name: GitBook Change Request
properties_list:
- description: The unique identifier of the change request.
  name: id
  type: string
- description: The sequential number of the change request.
  name: number
  type: integer
- description: The title or subject of the change request.
  name: subject
  type: string
- description: A description of the change request.
  name: description
  type: string
- description: The current status of the change request.
  name: status
  type: string
- description: The user who created the change request.
  name: createdBy
  type: object
- description: The timestamp when the change request was created.
  name: createdAt
  type: string
- description: The timestamp when the change request was last updated.
  name: updatedAt
  type: string
- description: The timestamp when the change request was merged, if applicable.
  name: mergedAt
  type: string
provider_name: GitBook
provider_slug: gitbook
schema_file: json-schema/change-request.json
slug: change-request
source_filename: change-request.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/gitbook/blob/main/json-schema/change-request.json\",\n  \"title\": \"GitBook Change Request\",\n  \"description\": \"A change request in GitBook represents a proposed set of content changes to a space, similar to a pull request. Change requests support collaborative review workflows before merging into the main content.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the change request.\"\n    },\n    \"number\": {\n      \"type\": \"integer\",\n      \"description\": \"The sequential number of the change request.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The title or subject of the change request.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the change request.\"\
  \n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"open\",\n        \"merged\",\n        \"closed\"\n      ],\n      \"description\": \"The current status of the change request.\"\n    },\n    \"createdBy\": {\n      \"$ref\": \"user.json\",\n      \"description\": \"The user who created the change request.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the change request was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the change request was last updated.\"\n    },\n    \"mergedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the change request was merged, if applicable.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/json-schema/change-request.json
tags:
- Content
- Documentation
- Experience
- Integrations
- Platform
- SDKs
title: GitBook Change Request
---
