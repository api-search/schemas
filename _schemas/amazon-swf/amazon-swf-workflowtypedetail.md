---
description: Contains details about a workflow type.
layout: schema
name: WorkflowTypeDetail
properties_list:
- description: ''
  name: typeInfo
  type: object
- description: ''
  name: configuration
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowtypedetail-schema.json
slug: amazon-swf-workflowtypedetail
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"typeInfo\",\n    \"configuration\"\n  ],\n  \"properties\": {\n    \"typeInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowTypeInfo\"\n        },\n        {\n          \"description\": \"<p>General information about the workflow type.</p> <p>The status of the workflow type (returned in the WorkflowTypeInfo structure) can be one of the following.</p> <ul> <li> <p> <code>REGISTERED</code> \\u2013 The type is registered and available. Workers supporting this type should be running.</p> </li> <li> <p> <code>DEPRECATED</code> \\u2013 The type was deprecated using <a>DeprecateWorkflowType</a>, but is still in use. You should keep workers supporting this type running. You cannot create new workflow executions of this type.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowTypeConfiguration\"\
  \n        },\n        {\n          \"description\": \"Configuration settings of the workflow type registered through <a>RegisterWorkflowType</a> \"\n        }\n      ]\n    }\n  },\n  \"description\": \"Contains details about a workflow type.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"WorkflowTypeDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowtypedetail-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: WorkflowTypeDetail
---
