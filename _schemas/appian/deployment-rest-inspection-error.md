---
description: An error identified during package inspection that would prevent successful deployment.
layout: schema
name: InspectionError
properties_list:
- description: A description of the error condition.
  name: errorMessage
  type: string
- description: The name of the object affected by the error.
  name: objectName
  type: string
- description: The UUID of the object affected by the error.
  name: objectUuid
  type: string
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-inspection-error-schema.json
slug: deployment-rest-inspection-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-inspection-error-schema.json\",\n  \"title\": \"InspectionError\",\n  \"description\": \"An error identified during package inspection that would prevent successful deployment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the error condition.\"\n    },\n    \"objectName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the object affected by the error.\"\n    },\n    \"objectUuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The UUID of the object affected by the error.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-inspection-error-schema.json
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: InspectionError
---
