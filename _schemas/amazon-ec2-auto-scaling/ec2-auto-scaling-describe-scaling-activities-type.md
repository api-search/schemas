---
description: DescribeScalingActivitiesType schema from Auto Scaling
layout: schema
name: DescribeScalingActivitiesType
properties_list:
- description: ''
  name: ActivityIds
  type: object
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: IncludeDeletedGroups
  type: object
- description: ''
  name: MaxRecords
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-describe-scaling-activities-type-schema.json
slug: ec2-auto-scaling-describe-scaling-activities-type
source_filename: ec2-auto-scaling-describe-scaling-activities-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-scaling-activities-type-schema.json\",\n  \"title\": \"DescribeScalingActivitiesType\",\n  \"description\": \"DescribeScalingActivitiesType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActivityIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityIds\"\n        },\n        {\n          \"description\": \"<p>The activity IDs of the desired scaling activities. If you omit this property, all activities for the past six weeks are described. If unknown activities are requested, they are ignored with no error. If you specify an Auto Scaling group, the results are limited to that group.</p> <p>Array Members: Maximum number of 50 IDs.</p>\"\n        }\n      ]\n    },\n    \"AutoScalingGroupName\": {\n \
  \     \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"IncludeDeletedGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IncludeDeletedGroups\"\n        },\n        {\n          \"description\": \"Indicates whether to include scaling activity from deleted Auto Scaling groups.\"\n        }\n      ]\n    },\n    \"MaxRecords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxRecords\"\n        },\n        {\n          \"description\": \"The maximum number of items to return with this call. The default value is <code>100</code> and the maximum value is <code>100</code>.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"\
  The token for the next set of items to return. (You received this token from a previous call.)\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-scaling-activities-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: DescribeScalingActivitiesType
---
