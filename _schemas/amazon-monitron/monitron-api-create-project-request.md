---
description: CreateProjectRequest schema from Amazon Monitron API
layout: schema
name: CreateProjectRequest
properties_list:
- description: A unique case-sensitive identifier used to idempotently create a resource.
  name: clientToken
  type: string
- description: The ID of the AWS Key Management Service (KMS) key to use to encrypt your project data.
  name: kmsKeyId
  type: string
- description: The name of the project.
  name: projectName
  type: string
- description: Resource tags to add to the project.
  name: tags
  type: object
provider_name: Amazon Monitron
provider_slug: amazon-monitron
schema_file: json-schema/monitron-api-create-project-request-schema.json
slug: monitron-api-create-project-request
source_filename: monitron-api-create-project-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-monitron/refs/heads/main/json-schema/monitron-api-create-project-request-schema.json\",\n  \"title\": \"CreateProjectRequest\",\n  \"description\": \"CreateProjectRequest schema from Amazon Monitron API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientToken\": {\n      \"description\": \"A unique case-sensitive identifier used to idempotently create a resource.\",\n      \"type\": \"string\"\n    },\n    \"kmsKeyId\": {\n      \"description\": \"The ID of the AWS Key Management Service (KMS) key to use to encrypt your project data.\",\n      \"type\": \"string\"\n    },\n    \"projectName\": {\n      \"description\": \"The name of the project.\",\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"description\": \"Resource tags to add to the project.\",\n      \"type\": \"object\"\n    }\n  },\n  \"required\": [\n \
  \   \"projectName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-monitron/refs/heads/main/json-schema/monitron-api-create-project-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CreateProjectRequest
---
