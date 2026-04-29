---
description: Represents a database script included in an export or import deployment.
layout: schema
name: DatabaseScript
properties_list:
- description: The file name of the database script.
  name: fileName
  type: string
- description: The execution order of the database script, starting at 1.
  name: orderId
  type: integer
- description: URL to download the database script file.
  name: url
  type: string
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-database-script-schema.json
slug: deployment-rest-database-script
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-database-script-schema.json\",\n  \"title\": \"DatabaseScript\",\n  \"description\": \"Represents a database script included in an export or import deployment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fileName\": {\n      \"type\": \"string\",\n      \"description\": \"The file name of the database script.\",\n      \"example\": \"create_tables.sql\"\n    },\n    \"orderId\": {\n      \"type\": \"integer\",\n      \"description\": \"The execution order of the database script, starting at 1.\",\n      \"minimum\": 1,\n      \"example\": 1\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to download the database script file.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-database-script-schema.json
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: DatabaseScript
---
