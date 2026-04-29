---
description: Represents a log source configured in Amazon Security Lake.
layout: schema
name: LogSource
properties_list:
- description: The name of the log source.
  name: sourceName
  type: string
- description: The version of the log source.
  name: sourceVersion
  type: string
- description: The status of the log source.
  name: sourceStatus
  type: string
provider_name: Amazon Security Lake
provider_slug: amazon-security-lake
schema_file: json-schema/amazon-security-lake-log-source-schema.json
slug: amazon-security-lake-log-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-security-lake/refs/heads/main/json-schema/amazon-security-lake-log-source-schema.json\",\n  \"title\": \"LogSource\",\n  \"description\": \"Represents a log source configured in Amazon Security Lake.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the log source.\",\n      \"example\": \"CLOUD_TRAIL_MGMT\"\n    },\n    \"sourceVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the log source.\",\n      \"example\": \"2.0\"\n    },\n    \"sourceStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the log source.\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"DEACTIVATED\",\n        \"PENDING\"\n      ],\n      \"example\": \"ACTIVE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-security-lake/refs/heads/main/json-schema/amazon-security-lake-log-source-schema.json
tags:
- AWS
- Data Lake
- Security
- SIEM
- Threat Detection
title: LogSource
---
