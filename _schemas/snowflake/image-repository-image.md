---
description: A image in a Snowflake image repository.
layout: schema
name: Image
properties_list:
- description: Date and time when the image was uploaded to the image repository.
  name: created_on
  type: string
- description: Image name.
  name: image_name
  type: string
- description: Image tags.
  name: tags
  type: string
- description: SHA256 digest of the image.
  name: digest
  type: string
- description: Image path (database_name/schema_name/repository_name/image_name:image_tag).
  name: image_path
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/image-repository-image-schema.json
slug: image-repository-image
source_filename: image-repository-image-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Image\",\n  \"type\": \"object\",\n  \"description\": \"A image in a Snowflake image repository.\",\n  \"properties\": {\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the image was uploaded to the image repository.\"\n    },\n    \"image_name\": {\n      \"type\": \"string\",\n      \"description\": \"Image name.\"\n    },\n    \"tags\": {\n      \"type\": \"string\",\n      \"description\": \"Image tags.\"\n    },\n    \"digest\": {\n      \"type\": \"string\",\n      \"description\": \"SHA256 digest of the image.\"\n    },\n    \"image_path\": {\n      \"type\": \"string\",\n      \"description\": \"Image path (database_name/schema_name/repository_name/image_name:image_tag).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/image-repository-image-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: Image
---
