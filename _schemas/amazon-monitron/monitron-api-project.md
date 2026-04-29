---
description: Represents a Monitron project.
layout: schema
name: Project
properties_list:
- description: The time at which the project was created.
  name: createdAt
  type: string
- description: The Amazon Resource Name (ARN) of the project.
  name: projectArn
  type: string
- description: The name of the project.
  name: projectName
  type: string
- description: The current status of the project.
  name: status
  type: string
- description: The time at which the project was last updated.
  name: updatedAt
  type: string
provider_name: Amazon Monitron
provider_slug: amazon-monitron
schema_file: json-schema/monitron-api-project-schema.json
slug: monitron-api-project
source_filename: monitron-api-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-monitron/refs/heads/main/json-schema/monitron-api-project-schema.json\",\n  \"title\": \"Project\",\n  \"description\": \"Represents a Monitron project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdAt\": {\n      \"description\": \"The time at which the project was created.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"projectArn\": {\n      \"description\": \"The Amazon Resource Name (ARN) of the project.\",\n      \"type\": \"string\"\n    },\n    \"projectName\": {\n      \"description\": \"The name of the project.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The current status of the project.\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"DELETING\"\n      ],\n      \"type\": \"string\"\n    },\n    \"updatedAt\": {\n      \"description\"\
  : \"The time at which the project was last updated.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-monitron/refs/heads/main/json-schema/monitron-api-project-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Project
---
