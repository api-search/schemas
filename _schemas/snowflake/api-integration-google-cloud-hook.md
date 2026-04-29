---
description: ''
layout: schema
name: GoogleCloudHook
properties_list:
- description: ''
  name: api_provider
  type: string
- description: Used as an audience claim when generating the JTW (JSON Web Token) to authenticate to the Google API Gateway.
  name: google_audience
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/api-integration-google-cloud-hook-schema.json
slug: api-integration-google-cloud-hook
source_filename: api-integration-google-cloud-hook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GoogleCloudHook\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"api_provider\": {\n      \"type\": \"string\"\n    },\n    \"google_audience\": {\n      \"type\": \"string\",\n      \"description\": \"Used as an audience claim when generating the JTW (JSON Web Token) to authenticate to the Google API Gateway.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/api-integration-google-cloud-hook-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: GoogleCloudHook
---
