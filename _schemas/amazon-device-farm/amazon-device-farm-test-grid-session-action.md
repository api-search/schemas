---
description: An action taken by a TestGridSession browser instance.
layout: schema
name: TestGridSessionAction
properties_list:
- description: ''
  name: action
  type: object
- description: ''
  name: started
  type: object
- description: ''
  name: duration
  type: object
- description: ''
  name: statusCode
  type: object
- description: ''
  name: requestMethod
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-test-grid-session-action-schema.json
slug: amazon-device-farm-test-grid-session-action
source_filename: amazon-device-farm-test-grid-session-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-test-grid-session-action-schema.json\",\n  \"title\": \"TestGridSessionAction\",\n  \"description\": \"An action taken by a TestGridSession browser instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The action taken by the session.\"\n        }\n      ]\n    },\n    \"started\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The time that the session invoked the action.\"\n        }\n      ]\n    },\n    \"duration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n  \
  \        \"description\": \"The time, in milliseconds, that the action took to complete in the browser.\"\n        }\n      ]\n    },\n    \"statusCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"HTTP status code returned to the browser when the action was taken.\"\n        }\n      ]\n    },\n    \"requestMethod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"HTTP method that the browser used to make the request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-test-grid-session-action-schema.json
tags:
- Application Testing
- AWS
- Device Testing
- Mobile Testing
- Quality Assurance
title: TestGridSessionAction
---
