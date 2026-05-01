---
description: ActivitiesType schema from Auto Scaling
layout: schema
name: ActivitiesType
properties_list:
- description: ''
  name: Activities
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-activities-type-schema.json
slug: ec2-auto-scaling-activities-type
source_filename: ec2-auto-scaling-activities-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-activities-type-schema.json\",\n  \"title\": \"ActivitiesType\",\n  \"description\": \"ActivitiesType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Activities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Activities\"\n        },\n        {\n          \"description\": \"The scaling activities. Activities are sorted by start time. Activities still in progress are described first.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"A string that indicates that the response contains more items than can be returned in a single response. To receive additional items, specify this\
  \ string for the <code>NextToken</code> value when requesting the next set of items. This value is null when there are no more items to return.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Activities\"\n  ],\n  \"example\": {\n    \"Activities\": [\n      {\n        \"ActivityId\": \"f9f2d65b-f1f2-43e7-b46d-d86756459699\",\n        \"AutoScalingGroupName\": \"my-auto-scaling-group\",\n        \"Cause\": \"At 2013-08-19T20:53:25Z a user request created an AutoScalingGroup changing the desired capacity from 0 to 1.  At 2013-08-19T20:53:29Z an instance was started in response to a difference between desired and actual capacity, increasing the capacity from 0 to 1.\",\n        \"Description\": \"Launching a new EC2 instance: i-4ba0837f\",\n        \"Details\": \"details\",\n        \"EndTime\": \"2013-08-19T20:54:02+00:00\",\n        \"Progress\": 100,\n        \"StartTime\": \"2013-08-19T20:53:29.930000+00:00\",\n        \"StatusCode\": \"Successful\"\n      }\n    ]\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-activities-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: ActivitiesType
---
