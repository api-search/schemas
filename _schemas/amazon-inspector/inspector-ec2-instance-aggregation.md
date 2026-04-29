---
description: The details that define an aggregation based on Amazon EC2 instances.
layout: schema
name: Ec2InstanceAggregation
properties_list:
- description: ''
  name: amis
  type: object
- description: ''
  name: instanceIds
  type: object
- description: ''
  name: instanceTags
  type: object
- description: ''
  name: operatingSystems
  type: object
- description: ''
  name: sortBy
  type: object
- description: ''
  name: sortOrder
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-ec2-instance-aggregation-schema.json
slug: inspector-ec2-instance-aggregation
source_filename: inspector-ec2-instance-aggregation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-ec2-instance-aggregation-schema.json\",\n  \"title\": \"Ec2InstanceAggregation\",\n  \"description\": \"The details that define an aggregation based on Amazon EC2 instances.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The AMI IDs associated with the Amazon EC2 instances to aggregate findings for.\"\n        }\n      ]\n    },\n    \"instanceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The Amazon EC2 instance IDs to aggregate findings for.\"\n        }\n      ]\n    },\n    \"instanceTags\": {\n      \"allOf\": [\n  \
  \      {\n          \"$ref\": \"#/components/schemas/MapFilterList\"\n        },\n        {\n          \"description\": \"The Amazon EC2 instance tags to aggregate findings for.\"\n        }\n      ]\n    },\n    \"operatingSystems\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The operating system types to aggregate findings for. Valid values must be uppercase and underscore separated, examples are <code>ORACLE_LINUX_7</code> and <code>ALPINE_LINUX_3_8</code>.\"\n        }\n      ]\n    },\n    \"sortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ec2InstanceSortBy\"\n        },\n        {\n          \"description\": \"The value to sort results by.\"\n        }\n      ]\n    },\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrder\"\n        },\n        {\n          \"description\": \"The order\
  \ to sort results by.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-ec2-instance-aggregation-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: Ec2InstanceAggregation
---
