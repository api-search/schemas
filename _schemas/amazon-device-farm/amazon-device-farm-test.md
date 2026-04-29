---
description: Represents a condition that is evaluated.
layout: schema
name: Test
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: created
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: result
  type: object
- description: ''
  name: started
  type: object
- description: ''
  name: stopped
  type: object
- description: ''
  name: counters
  type: object
- description: ''
  name: message
  type: object
- description: ''
  name: deviceMinutes
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-test-schema.json
slug: amazon-device-farm-test
source_filename: amazon-device-farm-test-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-test-schema.json\",\n  \"title\": \"Test\",\n  \"description\": \"Represents a condition that is evaluated.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The test's ARN.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The test's name.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TestType\"\n        },\n        {\n          \"description\": \"<p>The test's type.</p> <p>Must be one of the following values:</p>\
  \ <ul> <li> <p>BUILTIN_FUZZ</p> </li> <li> <p>BUILTIN_EXPLORER</p> <note> <p>For Android, an app explorer that traverses an Android app, interacting with it and capturing screenshots at the same time.</p> </note> </li> <li> <p>APPIUM_JAVA_JUNIT</p> </li> <li> <p>APPIUM_JAVA_TESTNG</p> </li> <li> <p>APPIUM_PYTHON</p> </li> <li> <p>APPIUM_NODE</p> </li> <li> <p>APPIUM_RUBY</p> </li> <li> <p>APPIUM_WEB_JAVA_JUNIT</p> </li> <li> <p>APPIUM_WEB_JAVA_TESTNG</p> </li> <li> <p>APPIUM_WEB_PYTHON</p> </li> <li> <p>APPIUM_WEB_NODE</p> </li> <li> <p>APPIUM_WEB_RUBY</p> </li> <li> <p>CALABASH</p> </li> <li> <p>INSTRUMENTATION</p> </li> <li> <p>UIAUTOMATION</p> </li> <li> <p>UIAUTOMATOR</p> </li> <li> <p>XCTEST</p> </li> <li> <p>XCTEST_UI</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"When the test was created.\"\n        }\n      ]\n    },\n  \
  \  \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionStatus\"\n        },\n        {\n          \"description\": \"<p>The test's status.</p> <p>Allowed values include:</p> <ul> <li> <p>PENDING</p> </li> <li> <p>PENDING_CONCURRENCY</p> </li> <li> <p>PENDING_DEVICE</p> </li> <li> <p>PROCESSING</p> </li> <li> <p>SCHEDULING</p> </li> <li> <p>PREPARING</p> </li> <li> <p>RUNNING</p> </li> <li> <p>COMPLETED</p> </li> <li> <p>STOPPING</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"result\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionResult\"\n        },\n        {\n          \"description\": \"<p>The test's result.</p> <p>Allowed values include:</p> <ul> <li> <p>PENDING</p> </li> <li> <p>PASSED</p> </li> <li> <p>WARNED</p> </li> <li> <p>FAILED</p> </li> <li> <p>SKIPPED</p> </li> <li> <p>ERRORED</p> </li> <li> <p>STOPPED</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"started\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The test's start time.\"\n        }\n      ]\n    },\n    \"stopped\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The test's stop time.\"\n        }\n      ]\n    },\n    \"counters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Counters\"\n        },\n        {\n          \"description\": \"The test's result counters.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"A message about the test's result.\"\n        }\n      ]\n    },\n    \"deviceMinutes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceMinutes\"\n        },\n        {\n          \"description\": \"Represents\
  \ the total (metered or unmetered) minutes used by the test.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-test-schema.json
tags:
- Application Testing
- AWS
- Device Testing
- Mobile Testing
- Quality Assurance
title: Test
---
