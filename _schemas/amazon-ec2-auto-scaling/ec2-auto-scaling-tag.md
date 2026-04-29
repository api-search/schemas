---
description: Describes a tag for an Auto Scaling group.
layout: schema
name: Tag
properties_list:
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: ResourceType
  type: object
- description: ''
  name: Key
  type: object
- description: ''
  name: Value
  type: object
- description: ''
  name: PropagateAtLaunch
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-tag-schema.json
slug: ec2-auto-scaling-tag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"Describes a tag for an Auto Scaling group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"ResourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"The type of resource. The only supported value is <code>auto-scaling-group</code>.\"\n        }\n      ]\n    },\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKey\"\n        },\n        {\n\
  \          \"description\": \"The tag key.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagValue\"\n        },\n        {\n          \"description\": \"The tag value.\"\n        }\n      ]\n    },\n    \"PropagateAtLaunch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropagateAtLaunch\"\n        },\n        {\n          \"description\": \"Determines whether the tag is added to new instances as they are launched in the group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-tag-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: Tag
---
