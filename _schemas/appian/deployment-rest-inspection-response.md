---
description: Response returned when an inspection operation is successfully initiated. Contains the UUID for tracking the inspection.
layout: schema
name: InspectionResponse
properties_list:
- description: Unique identifier for the inspection operation. Use this UUID to retrieve inspection results.
  name: uuid
  type: string
- description: URL endpoint for retrieving the inspection details and results.
  name: url
  type: string
provider_name: Appian
provider_slug: appian
schema_file: json-schema/deployment-rest-inspection-response-schema.json
slug: deployment-rest-inspection-response
source_filename: deployment-rest-inspection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-inspection-response-schema.json\",\n  \"title\": \"InspectionResponse\",\n  \"description\": \"Response returned when an inspection operation is successfully initiated. Contains the UUID for tracking the inspection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the inspection operation. Use this UUID to retrieve inspection results.\",\n      \"example\": \"378271a6-ca0d-4466-bac9-385e4fcb951a\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL endpoint for retrieving the inspection details and results.\",\n      \"example\": \"https://mysite.appiancloud.com/suite/deployment-management/v2/inspections/378271a6-ca0d-4466-bac9-385e4fcb951a/\"\
  \n    }\n  },\n  \"required\": [\n    \"uuid\",\n    \"url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/deployment-rest-inspection-response-schema.json
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: InspectionResponse
---
