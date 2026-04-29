---
description: A system registered in QueryGrid.
layout: schema
name: System
properties_list:
- description: Unique system identifier.
  name: id
  type: string
- description: System name.
  name: name
  type: string
- description: System type.
  name: type
  type: string
- description: Parent data center identifier.
  name: dataCenterId
  type: string
- description: System status.
  name: status
  type: string
- description: System hostname.
  name: hostname
  type: string
provider_name: Teradata
provider_slug: teradata
schema_file: json-schema/querygrid-manager-api-system-schema.json
slug: querygrid-manager-api-system
source_filename: querygrid-manager-api-system-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/querygrid-manager-api-system-schema.json\",\n  \"title\": \"System\",\n  \"description\": \"A system registered in QueryGrid.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique system identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"System name.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"System type.\",\n      \"enum\": [\"teradata\", \"hadoop\", \"spark\", \"hive\", \"presto\", \"oracle\"]\n    },\n    \"dataCenterId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent data center identifier.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"System status.\"\n    },\n    \"hostname\": {\n      \"type\": \"\
  string\",\n      \"description\": \"System hostname.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/querygrid-manager-api-system-schema.json
tags:
- Analytics
- Cloud
- Data Management
- Data Warehousing
- Database
- Enterprise
- Machine Learning
- SQL
title: System
---
