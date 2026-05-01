---
description: DescribeActivityOutput schema from Amazon Step Functions API
layout: schema
name: DescribeActivityOutput
properties_list:
- description: ''
  name: activityArn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: creationDate
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-describe-activity-output-schema.json
slug: amazon-step-functions-describe-activity-output
source_filename: amazon-step-functions-describe-activity-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-activity-output-schema.json\",\n  \"title\": \"DescribeActivityOutput\",\n  \"description\": \"DescribeActivityOutput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"activityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) that identifies the activity.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"<p>The name of the activity.</p> <p>A name must <i>not</i> contain:</p> <ul> <li> <p>white space</p> </li> <li> <p>brackets <code>&lt; &gt; { } [ ]</code> </p> </li> <li>\
  \ <p>wildcard characters <code>? *</code> </p> </li> <li> <p>special characters <code>\\\" # % \\\\ ^ | ~ ` $ &amp; , ; : /</code> </p> </li> <li> <p>control characters (<code>U+0000-001F</code>, <code>U+007F-009F</code>)</p> </li> </ul> <p>To enable logging with CloudWatch Logs, the name should only contain 0-9, A-Z, a-z, - and _.</p>\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date the activity is created.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"activityArn\",\n    \"name\",\n    \"creationDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-describe-activity-output-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: DescribeActivityOutput
---
