---
description: DescribeInstanceRefreshesAnswer schema from Auto Scaling
layout: schema
name: DescribeInstanceRefreshesAnswer
properties_list:
- description: ''
  name: InstanceRefreshes
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-describe-instance-refreshes-answer-schema.json
slug: ec2-auto-scaling-describe-instance-refreshes-answer
source_filename: ec2-auto-scaling-describe-instance-refreshes-answer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-instance-refreshes-answer-schema.json\",\n  \"title\": \"DescribeInstanceRefreshesAnswer\",\n  \"description\": \"DescribeInstanceRefreshesAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceRefreshes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceRefreshes\"\n        },\n        {\n          \"description\": \"The instance refreshes for the specified group, sorted by creation timestamp in descending order.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"A string that indicates that the response contains more items than can be returned in a single\
  \ response. To receive additional items, specify this string for the <code>NextToken</code> value when requesting the next set of items. This value is null when there are no more items to return.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"InstanceRefreshes\": [\n      {\n        \"AutoScalingGroupName\": \"my-auto-scaling-group\",\n        \"InstanceRefreshId\": \"08b91cf7-8fa6-48af-b6a6-d227f40f1b9b\",\n        \"InstancesToUpdate\": 5,\n        \"PercentageComplete\": 0,\n        \"StartTime\": \"2020-06-02T18:11:27+00:00\",\n        \"Status\": \"InProgress\"\n      },\n      {\n        \"AutoScalingGroupName\": \"my-auto-scaling-group\",\n        \"EndTime\": \"2020-06-02T16:53:37+00:00\",\n        \"InstanceRefreshId\": \"dd7728d0-5bc4-4575-96a3-1b2c52bf8bb1\",\n        \"InstancesToUpdate\": 0,\n        \"PercentageComplete\": 100,\n        \"StartTime\": \"2020-06-02T16:43:19+00:00\",\n        \"Status\": \"Successful\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-describe-instance-refreshes-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: DescribeInstanceRefreshesAnswer
---
