---
description: A TestGridSession is a single instance of a browser launched from the URL provided by a call to CreateTestGridUrl.
layout: schema
name: TestGridSession
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: created
  type: object
- description: ''
  name: ended
  type: object
- description: ''
  name: billingMinutes
  type: object
- description: ''
  name: seleniumProperties
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-test-grid-session-schema.json
slug: amazon-device-farm-test-grid-session
source_filename: amazon-device-farm-test-grid-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-test-grid-session-schema.json\",\n  \"title\": \"TestGridSession\",\n  \"description\": \"A TestGridSession is a single instance of a browser launched from the URL provided by a call to CreateTestGridUrl.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceFarmArn\"\n        },\n        {\n          \"description\": \"The ARN of the session.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TestGridSessionStatus\"\n        },\n        {\n          \"description\": \"The state of the session.\"\n        }\n      ]\n    },\n    \"created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\
  \n        },\n        {\n          \"description\": \"The time that the session was started.\"\n        }\n      ]\n    },\n    \"ended\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The time the session ended.\"\n        }\n      ]\n    },\n    \"billingMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"The number of billed minutes that were used for this session. \"\n        }\n      ]\n    },\n    \"seleniumProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A JSON object of options and parameters passed to the Selenium WebDriver.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-test-grid-session-schema.json
tags:
- Application Testing
- AWS
- Device Testing
- Mobile Testing
- Quality Assurance
title: TestGridSession
---
