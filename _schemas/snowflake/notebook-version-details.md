---
description: The version details of a file based entity
layout: schema
name: VersionDetails
properties_list:
- description: The last version name
  name: name
  type: string
- description: The default/last version alias of a file based entity.
  name: alias
  type: string
- description: The default/last version location.
  name: location_url
  type: string
- description: The default/last version source location.
  name: source_location_uri
  type: string
- description: The default/last version git commit#
  name: git_commit_hash
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/notebook-version-details-schema.json
slug: notebook-version-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VersionDetails\",\n  \"type\": \"object\",\n  \"description\": \"The version details of a file based entity\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The last version name\"\n    },\n    \"alias\": {\n      \"type\": \"string\",\n      \"description\": \"The default/last version alias of a file based entity.\"\n    },\n    \"location_url\": {\n      \"type\": \"string\",\n      \"description\": \"The default/last version location.\"\n    },\n    \"source_location_uri\": {\n      \"type\": \"string\",\n      \"description\": \"The default/last version source location.\"\n    },\n    \"git_commit_hash\": {\n      \"type\": \"string\",\n      \"description\": \"The default/last version git commit#\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/notebook-version-details-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: VersionDetails
---
