---
description: A Snowflake image repository.
layout: schema
name: ImageRepository
properties_list:
- description: Time the image repository was created.
  name: created_on
  type: string
- description: Current URL of the image repository.
  name: repository_url
  type: string
- description: Identifier for the current owner of the image repository.
  name: owner
  type: string
- description: Role type of the image repository owner.
  name: owner_role_type
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/image-repository-image-repository-schema.json
slug: image-repository-image-repository
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImageRepository\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake image repository.\",\n  \"properties\": {\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Time the image repository was created.\"\n    },\n    \"repository_url\": {\n      \"type\": \"string\",\n      \"description\": \"Current URL of the image repository.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for the current owner of the image repository.\"\n    },\n    \"owner_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"Role type of the image repository owner.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/image-repository-image-repository-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ImageRepository
---
