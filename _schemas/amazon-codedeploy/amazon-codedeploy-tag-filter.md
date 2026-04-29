---
description: Information about an on-premises instance tag filter.
layout: schema
name: TagFilter
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
schema_file: json-schema/amazon-codedeploy-tag-filter-schema.json
slug: amazon-codedeploy-tag-filter
source_filename: amazon-codedeploy-tag-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-tag-filter-schema.json\",\n  \"title\": \"TagFilter\",\n  \"description\": \"Information about an on-premises instance tag filter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Key\"\n        },\n        {\n          \"description\": \"The on-premises instance tag filter key.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Value\"\n        },\n        {\n          \"description\": \"The on-premises instance tag filter value.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagFilterType\"\n        },\n        {\n          \"description\": \"<p>The\
  \ on-premises instance tag filter type:</p> <ul> <li> <p>KEY_ONLY: Key only.</p> </li> <li> <p>VALUE_ONLY: Value only.</p> </li> <li> <p>KEY_AND_VALUE: Key and value.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-tag-filter-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: TagFilter
---
