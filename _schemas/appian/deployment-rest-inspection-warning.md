---
description: A warning identified during package inspection that may affect deployment but would not prevent it.
layout: schema
name: InspectionWarning
properties_list:
- description: A description of the warning condition.
  name: warningMessage
  type: string
- description: The name of the object associated with the warning.
  name: objectName
  type: string
- description: The UUID of the object associated with the warning.
  name: objectUuid
  type: string
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-inspection-warning-schema.json
slug: deployment-rest-inspection-warning
source_filename: deployment-rest-inspection-warning-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-inspection-warning-schema.json\",\n  \"title\": \"InspectionWarning\",\n  \"description\": \"A warning identified during package inspection that may affect deployment but would not prevent it.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"warningMessage\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the warning condition.\"\n    },\n    \"objectName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the object associated with the warning.\"\n    },\n    \"objectUuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The UUID of the object associated with the warning.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-inspection-warning-schema.json
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: InspectionWarning
---
