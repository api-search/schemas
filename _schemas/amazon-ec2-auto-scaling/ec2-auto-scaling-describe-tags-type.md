---
description: DescribeTagsType schema from Auto Scaling
layout: schema
name: DescribeTagsType
properties_list:
- description: ''
  name: Filters
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxRecords
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-describe-tags-type-schema.json
slug: ec2-auto-scaling-describe-tags-type
source_filename: ec2-auto-scaling-describe-tags-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-tags-type-schema.json\",\n  \"title\": \"DescribeTagsType\",\n  \"description\": \"DescribeTagsType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Filters\"\n        },\n        {\n          \"description\": \"One or more filters to scope the tags to return. The maximum number of filters per filter type (for example, <code>auto-scaling-group</code>) is 1000.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"The token for the next set of items to return. (You received this token from a previous call.)\"\n     \
  \   }\n      ]\n    },\n    \"MaxRecords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxRecords\"\n        },\n        {\n          \"description\": \"The maximum number of items to return with this call. The default value is <code>50</code> and the maximum value is <code>100</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-tags-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: DescribeTagsType
---
