---
description: Used to filter workflow execution query results by type. Each parameter, if specified, defines a rule that must be satisfied by each returned result.
layout: schema
name: WorkflowTypeFilter
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: version
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowtypefilter-schema.json
slug: amazon-swf-workflowtypefilter
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \" Name of the workflow type.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionOptional\"\n        },\n        {\n          \"description\": \"Version of the workflow type.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Used to filter workflow execution query results by type. Each parameter, if specified, defines a rule that must be satisfied by each returned result.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"WorkflowTypeFilter\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowtypefilter-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: WorkflowTypeFilter
---
