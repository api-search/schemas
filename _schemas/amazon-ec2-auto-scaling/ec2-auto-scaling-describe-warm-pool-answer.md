---
description: DescribeWarmPoolAnswer schema from Auto Scaling
layout: schema
name: DescribeWarmPoolAnswer
properties_list:
- description: ''
  name: WarmPoolConfiguration
  type: object
- description: ''
  name: Instances
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-describe-warm-pool-answer-schema.json
slug: ec2-auto-scaling-describe-warm-pool-answer
source_filename: ec2-auto-scaling-describe-warm-pool-answer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-warm-pool-answer-schema.json\",\n  \"title\": \"DescribeWarmPoolAnswer\",\n  \"description\": \"DescribeWarmPoolAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"WarmPoolConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WarmPoolConfiguration\"\n        },\n        {\n          \"description\": \"The warm pool configuration details. \"\n        }\n      ]\n    },\n    \"Instances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Instances\"\n        },\n        {\n          \"description\": \"The instances that are currently in the warm pool.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\
  \n        },\n        {\n          \"description\": \"This string indicates that the response contains more items than can be returned in a single response. To receive additional items, specify this string for the <code>NextToken</code> value when requesting the next set of items. This value is null when there are no more items to return.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-warm-pool-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: DescribeWarmPoolAnswer
---
