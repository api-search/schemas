---
description: ''
layout: schema
name: DescribeActivityTypeInput
properties_list:
- description: ''
  name: domain
  type: object
- description: ''
  name: activityType
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-describeactivitytypeinput-schema.json
slug: amazon-swf-describeactivitytypeinput
source_filename: amazon-swf-describeactivitytypeinput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\",\n    \"activityType\"\n  ],\n  \"title\": \"DescribeActivityTypeInput\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain in which the activity type is registered.\"\n        }\n      ]\n    },\n    \"activityType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityType\"\n        },\n        {\n          \"description\": \"The activity type to get information about. Activity types are identified by the <code>name</code> and <code>version</code> that were supplied when the activity was registered.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-describeactivitytypeinput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: DescribeActivityTypeInput
---
