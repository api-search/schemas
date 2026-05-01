---
description: Information about active sessions for a Dev Environment.
layout: schema
name: DevEnvironmentSessionSummary
properties_list:
- description: ''
  name: spaceName
  type: object
- description: ''
  name: projectName
  type: object
- description: ''
  name: devEnvironmentId
  type: object
- description: ''
  name: startedTime
  type: object
- description: ''
  name: id
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-dev-environment-session-summary-schema.json
slug: amazon-codecatalyst-dev-environment-session-summary
source_filename: amazon-codecatalyst-dev-environment-session-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-dev-environment-session-summary-schema.json\",\n  \"title\": \"DevEnvironmentSessionSummary\",\n  \"description\": \"Information about active sessions for a Dev Environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"spaceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the space.\"\n        }\n      ]\n    },\n    \"projectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the project in the space.\"\n        }\n      ]\n    },\n    \"devEnvironmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n    \
  \    },\n        {\n          \"description\": \"The system-generated unique ID of the Dev Environment.\"\n        }\n      ]\n    },\n    \"startedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"The date and time the session started, in coordinated universal time (UTC) timestamp format as specified in <a href=\\\"https://www.rfc-editor.org/rfc/rfc3339#section-5.6\\\">RFC 3339</a> \"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevEnvironmentSessionSummaryIdString\"\n        },\n        {\n          \"description\": \"The system-generated unique ID of the Dev Environment session.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"spaceName\",\n    \"projectName\",\n    \"devEnvironmentId\",\n    \"startedTime\",\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-dev-environment-session-summary-schema.json
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: DevEnvironmentSessionSummary
---
