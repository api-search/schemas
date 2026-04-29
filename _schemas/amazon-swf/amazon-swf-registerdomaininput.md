---
description: ''
layout: schema
name: RegisterDomainInput
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: workflowExecutionRetentionPeriodInDays
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-registerdomaininput-schema.json
slug: amazon-swf-registerdomaininput
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"workflowExecutionRetentionPeriodInDays\"\n  ],\n  \"title\": \"RegisterDomainInput\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"<p>Name of the domain to register. The name must be unique in the region that the domain is registered in.</p> <p>The specified string must not start or end with whitespace. It must not contain a <code>:</code> (colon), <code>/</code> (slash), <code>|</code> (vertical bar), or any control characters (<code>\\\\u0000-\\\\u001f</code> | <code>\\\\u007f-\\\\u009f</code>). Also, it must <i>not</i> be the literal string <code>arn</code>.</p>\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A text description\
  \ of the domain.\"\n        }\n      ]\n    },\n    \"workflowExecutionRetentionPeriodInDays\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInDays\"\n        },\n        {\n          \"description\": \"<p>The duration (in days) that records and histories of workflow executions on the domain should be kept by the service. After the retention period, the workflow execution isn't available in the results of visibility calls.</p> <p>If you pass the value <code>NONE</code> or <code>0</code> (zero), then the workflow execution history isn't retained. As soon as the workflow execution completes, the execution record and its history are deleted.</p> <p>The maximum workflow execution retention period is 90 days. For more information about Amazon SWF service limits, see: <a href=\\\"https://docs.aws.amazon.com/amazonswf/latest/developerguide/swf-dg-limits.html\\\">Amazon SWF Service Limits</a> in the <i>Amazon SWF Developer Guide</i>.</p>\"\n        }\n \
  \     ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTagList\"\n        },\n        {\n          \"description\": \"<p>Tags to be added when registering a domain.</p> <p>Tags may only contain unicode letters, digits, whitespace, or these symbols: <code>_ . : / = + - @</code>.</p>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-registerdomaininput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: RegisterDomainInput
---
