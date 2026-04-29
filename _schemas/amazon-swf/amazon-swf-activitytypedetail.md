---
description: Detailed information about an activity type.
layout: schema
name: ActivityTypeDetail
properties_list:
- description: ''
  name: typeInfo
  type: object
- description: ''
  name: configuration
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-activitytypedetail-schema.json
slug: amazon-swf-activitytypedetail
source_filename: amazon-swf-activitytypedetail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"typeInfo\",\n    \"configuration\"\n  ],\n  \"properties\": {\n    \"typeInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityTypeInfo\"\n        },\n        {\n          \"description\": \"<p>General information about the activity type.</p> <p>The status of activity type (returned in the ActivityTypeInfo structure) can be one of the following.</p> <ul> <li> <p> <code>REGISTERED</code> \\u2013 The type is registered and available. Workers supporting this type should be running. </p> </li> <li> <p> <code>DEPRECATED</code> \\u2013 The type was deprecated using <a>DeprecateActivityType</a>, but is still in use. You should keep workers supporting this type running. You cannot create new tasks of this type. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityTypeConfiguration\"\n     \
  \   },\n        {\n          \"description\": \"The configuration settings registered with the activity type.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Detailed information about an activity type.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ActivityTypeDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-activitytypedetail-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: ActivityTypeDetail
---
