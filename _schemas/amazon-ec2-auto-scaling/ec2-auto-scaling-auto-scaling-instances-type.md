---
description: AutoScalingInstancesType schema from Auto Scaling
layout: schema
name: AutoScalingInstancesType
properties_list:
- description: ''
  name: AutoScalingInstances
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-auto-scaling-instances-type-schema.json
slug: ec2-auto-scaling-auto-scaling-instances-type
source_filename: ec2-auto-scaling-auto-scaling-instances-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-auto-scaling-instances-type-schema.json\",\n  \"title\": \"AutoScalingInstancesType\",\n  \"description\": \"AutoScalingInstancesType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingInstances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingInstances\"\n        },\n        {\n          \"description\": \"The instances.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"A string that indicates that the response contains more items than can be returned in a single response. To receive additional items, specify this string for the <code>NextToken</code> value\
  \ when requesting the next set of items. This value is null when there are no more items to return.\"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"AutoScalingInstances\": [\n      {\n        \"AutoScalingGroupName\": \"my-auto-scaling-group\",\n        \"AvailabilityZone\": \"us-west-2c\",\n        \"HealthStatus\": \"HEALTHY\",\n        \"InstanceId\": \"i-4ba0837f\",\n        \"LaunchConfigurationName\": \"my-launch-config\",\n        \"LifecycleState\": \"InService\",\n        \"ProtectedFromScaleIn\": false\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-auto-scaling-instances-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: AutoScalingInstancesType
---
