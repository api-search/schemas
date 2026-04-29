---
description: Request body for creating a package inspection operation. Requires the deployment package and Admin Console settings files, with an optional import customization file.
layout: schema
name: InspectionRequest
properties_list:
- description: JSON string containing the inspection configuration with file name references for the attached files.
  name: json
  type: string
- description: Admin Console settings ZIP file to use for the inspection.
  name: adminConsoleSettingsFileName
  type: string
- description: The deployment package ZIP file to inspect.
  name: packageFileName
  type: string
- description: Optional import customization properties file to include in the inspection.
  name: customizationFileName
  type: string
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-inspection-request-schema.json
slug: deployment-rest-inspection-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-inspection-request-schema.json\",\n  \"title\": \"InspectionRequest\",\n  \"description\": \"Request body for creating a package inspection operation. Requires the deployment package and Admin Console settings files, with an optional import customization file.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"json\": {\n      \"type\": \"string\",\n      \"description\": \"JSON string containing the inspection configuration with file name references for the attached files.\"\n    },\n    \"adminConsoleSettingsFileName\": {\n      \"type\": \"string\",\n      \"format\": \"binary\",\n      \"description\": \"Admin Console settings ZIP file to use for the inspection.\"\n    },\n    \"packageFileName\": {\n      \"type\": \"string\",\n      \"format\": \"binary\",\n      \"description\": \"The\
  \ deployment package ZIP file to inspect.\"\n    },\n    \"customizationFileName\": {\n      \"type\": \"string\",\n      \"format\": \"binary\",\n      \"description\": \"Optional import customization properties file to include in the inspection.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-inspection-request-schema.json
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: InspectionRequest
---
