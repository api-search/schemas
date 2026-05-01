---
description: TagsType schema from Auto Scaling
layout: schema
name: TagsType
properties_list:
- description: ''
  name: Tags
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-tags-type-schema.json
slug: ec2-auto-scaling-tags-type
source_filename: ec2-auto-scaling-tags-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-tags-type-schema.json\",\n  \"title\": \"TagsType\",\n  \"description\": \"TagsType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagDescriptionList\"\n        },\n        {\n          \"description\": \"One or more tags.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"A string that indicates that the response contains more items than can be returned in a single response. To receive additional items, specify this string for the <code>NextToken</code> value when requesting the next set of items. This value is null when\
  \ there are no more items to return.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"Tags\": [\n      {\n        \"Key\": \"Dept\",\n        \"PropagateAtLaunch\": true,\n        \"ResourceId\": \"my-auto-scaling-group\",\n        \"ResourceType\": \"auto-scaling-group\",\n        \"Value\": \"Research\"\n      },\n      {\n        \"Key\": \"Role\",\n        \"PropagateAtLaunch\": true,\n        \"ResourceId\": \"my-auto-scaling-group\",\n        \"ResourceType\": \"auto-scaling-group\",\n        \"Value\": \"WebServer\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-tags-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: TagsType
---
