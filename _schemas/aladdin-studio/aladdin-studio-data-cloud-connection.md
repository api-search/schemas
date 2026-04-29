---
description: An Aladdin Data Cloud Snowflake connection
layout: schema
name: Connection
properties_list:
- description: Unique connection identifier
  name: connectionId
  type: string
- description: Snowflake account URL
  name: accountName
  type: string
- description: Snowflake database name
  name: database
  type: string
- description: Snowflake virtual warehouse
  name: warehouse
  type: string
- description: Connection status
  name: status
  type: string
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-data-cloud-connection-schema.json
slug: aladdin-studio-data-cloud-connection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-data-cloud-connection-schema.json\",\n  \"title\": \"Connection\",\n  \"description\": \"An Aladdin Data Cloud Snowflake connection\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique connection identifier\",\n      \"example\": \"adc-conn-001\"\n    },\n    \"accountName\": {\n      \"type\": \"string\",\n      \"description\": \"Snowflake account URL\",\n      \"example\": \"blackrock.snowflakecomputing.com\"\n    },\n    \"database\": {\n      \"type\": \"string\",\n      \"description\": \"Snowflake database name\",\n      \"example\": \"ALADDIN_DATA_CLOUD\"\n    },\n    \"warehouse\": {\n      \"type\": \"string\",\n      \"description\": \"Snowflake virtual warehouse\",\n      \"example\": \"ANALYTICS_WH\"\
  \n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Connection status\",\n      \"enum\": [\n        \"active\",\n        \"inactive\"\n      ],\n      \"example\": \"active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-data-cloud-connection-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: Connection
---
