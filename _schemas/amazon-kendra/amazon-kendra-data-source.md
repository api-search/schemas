---
description: A data source connector for an Amazon Kendra index.
layout: schema
name: DataSource
properties_list:
- description: The identifier of the data source.
  name: Id
  type: string
- description: The name of the data source.
  name: Name
  type: string
- description: The type of the data source.
  name: Type
  type: string
- description: The status of the data source.
  name: Status
  type: string
- description: The cron schedule for sync.
  name: Schedule
  type: string
- description: The ID of the index this data source belongs to.
  name: IndexId
  type: string
provider_name: Amazon Kendra
provider_slug: amazon-kendra
schema_file: json-schema/amazon-kendra-data-source-schema.json
slug: amazon-kendra-data-source
source_filename: amazon-kendra-data-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/json-schema/amazon-kendra-data-source-schema.json\",\n  \"title\": \"DataSource\",\n  \"description\": \"A data source connector for an Amazon Kendra index.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the data source.\",\n      \"example\": \"ds-abc12345\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the data source.\",\n      \"example\": \"sharepoint-connector\"\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"S3\",\n        \"SHAREPOINT\",\n        \"DATABASE\",\n        \"SALESFORCE\",\n        \"ONEDRIVE\",\n        \"SERVICENOW\",\n        \"CUSTOM\",\n        \"CONFLUENCE\",\n        \"GOOGLEDRIVE\",\n        \"WEBCRAWLER\",\n        \"\
  WORKDOCS\"\n      ],\n      \"description\": \"The type of the data source.\",\n      \"example\": \"S3\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CREATING\",\n        \"DELETING\",\n        \"FAILED\",\n        \"UPDATING\",\n        \"ACTIVE\"\n      ],\n      \"description\": \"The status of the data source.\",\n      \"example\": \"ACTIVE\"\n    },\n    \"Schedule\": {\n      \"type\": \"string\",\n      \"description\": \"The cron schedule for sync.\",\n      \"example\": \"cron(0 11 * * ? *)\"\n    },\n    \"IndexId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the index this data source belongs to.\",\n      \"example\": \"abc12345-6789-def0-1234-abcdef012345\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-kendra/refs/heads/main/json-schema/amazon-kendra-data-source-schema.json
tags:
- AI
- AWS
- Enterprise Search
- Knowledge Management
- Machine Learning
- Natural Language
title: DataSource
---
