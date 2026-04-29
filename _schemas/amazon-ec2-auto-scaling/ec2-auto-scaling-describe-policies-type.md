---
description: DescribePoliciesType schema from Auto Scaling
layout: schema
name: DescribePoliciesType
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: PolicyNames
  type: object
- description: ''
  name: PolicyTypes
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxRecords
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-describe-policies-type-schema.json
slug: ec2-auto-scaling-describe-policies-type
source_filename: ec2-auto-scaling-describe-policies-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-policies-type-schema.json\",\n  \"title\": \"DescribePoliciesType\",\n  \"description\": \"DescribePoliciesType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"PolicyNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyNames\"\n        },\n        {\n          \"description\": \"<p>The names of one or more policies. If you omit this property, all policies are described. If a group name is provided, the results are limited to that group. If you specify an\
  \ unknown policy name, it is ignored with no error.</p> <p>Array Members: Maximum number of 50 items.</p>\"\n        }\n      ]\n    },\n    \"PolicyTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyTypes\"\n        },\n        {\n          \"description\": \"One or more policy types. The valid values are <code>SimpleScaling</code>, <code>StepScaling</code>, <code>TargetTrackingScaling</code>, and <code>PredictiveScaling</code>.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"The token for the next set of items to return. (You received this token from a previous call.)\"\n        }\n      ]\n    },\n    \"MaxRecords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxRecords\"\n        },\n        {\n          \"description\": \"The maximum number of items to be returned with\
  \ each call. The default value is <code>50</code> and the maximum value is <code>100</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-policies-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: DescribePoliciesType
---
