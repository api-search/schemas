---
description: Information about an EC2 tag filter.
layout: schema
name: EC2TagFilter
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Value
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-ec2-tag-filter-schema.json
slug: amazon-codedeploy-ec2-tag-filter
source_filename: amazon-codedeploy-ec2-tag-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-ec2-tag-filter-schema.json\",\n  \"title\": \"EC2TagFilter\",\n  \"description\": \"Information about an EC2 tag filter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Key\"\n        },\n        {\n          \"description\": \"The tag filter key.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Value\"\n        },\n        {\n          \"description\": \"The tag filter value.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2TagFilterType\"\n        },\n        {\n          \"description\": \"<p>The tag filter type:</p> <ul> <li> <p> <code>KEY_ONLY</code>:\
  \ Key only.</p> </li> <li> <p> <code>VALUE_ONLY</code>: Value only.</p> </li> <li> <p> <code>KEY_AND_VALUE</code>: Key and value.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-ec2-tag-filter-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: EC2TagFilter
---
