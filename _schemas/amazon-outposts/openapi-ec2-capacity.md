---
description: Information about EC2 capacity.
layout: schema
name: EC2Capacity
properties_list:
- description: ''
  name: Family
  type: object
- description: ''
  name: MaxSize
  type: object
- description: ''
  name: Quantity
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-ec2-capacity-schema.json
slug: openapi-ec2-capacity
source_filename: openapi-ec2-capacity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-ec2-capacity-schema.json\",\n  \"title\": \"EC2Capacity\",\n  \"description\": \" Information about EC2 capacity. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Family\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Family\"\n        },\n        {\n          \"description\": \" The family of the EC2 capacity. \"\n        }\n      ]\n    },\n    \"MaxSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxSize\"\n        },\n        {\n          \"description\": \" The maximum size of the EC2 capacity. \"\n        }\n      ]\n    },\n    \"Quantity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Quantity\"\n        },\n        {\n          \"description\": \" The quantity of the EC2 capacity.\
  \ \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-ec2-capacity-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: EC2Capacity
---
