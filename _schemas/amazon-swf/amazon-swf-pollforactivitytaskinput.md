---
description: ''
layout: schema
name: PollForActivityTaskInput
properties_list:
- description: ''
  name: domain
  type: object
- description: ''
  name: taskList
  type: object
- description: ''
  name: identity
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-pollforactivitytaskinput-schema.json
slug: amazon-swf-pollforactivitytaskinput
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\",\n    \"taskList\"\n  ],\n  \"title\": \"PollForActivityTaskInput\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain that contains the task lists being polled.\"\n        }\n      ]\n    },\n    \"taskList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskList\"\n        },\n        {\n          \"description\": \"<p>Specifies the task list to poll for activity tasks.</p> <p>The specified string must not start or end with whitespace. It must not contain a <code>:</code> (colon), <code>/</code> (slash), <code>|</code> (vertical bar), or any control characters (<code>\\\\u0000-\\\\u001f</code> | <code>\\\\u007f-\\\\u009f</code>). Also, it must <i>not</i> be the literal string <code>arn</code>.</p>\"\n        }\n      ]\n    },\n\
  \    \"identity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identity\"\n        },\n        {\n          \"description\": \"Identity of the worker making the request, recorded in the <code>ActivityTaskStarted</code> event in the workflow history. This enables diagnostic tracing when problems arise. The form of this identity is user defined.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-pollforactivitytaskinput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: PollForActivityTaskInput
---
