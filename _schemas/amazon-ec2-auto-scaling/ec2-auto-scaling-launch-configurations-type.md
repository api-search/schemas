---
description: LaunchConfigurationsType schema from Auto Scaling
layout: schema
name: LaunchConfigurationsType
properties_list:
- description: ''
  name: LaunchConfigurations
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-launch-configurations-type-schema.json
slug: ec2-auto-scaling-launch-configurations-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-launch-configurations-type-schema.json\",\n  \"title\": \"LaunchConfigurationsType\",\n  \"description\": \"LaunchConfigurationsType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LaunchConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchConfigurations\"\n        },\n        {\n          \"description\": \"The launch configurations.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"A string that indicates that the response contains more items than can be returned in a single response. To receive additional items, specify this string for the <code>NextToken</code>\
  \ value when requesting the next set of items. This value is null when there are no more items to return.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LaunchConfigurations\"\n  ],\n  \"example\": {\n    \"LaunchConfigurations\": [\n      {\n        \"AssociatePublicIpAddress\": true,\n        \"BlockDeviceMappings\": [],\n        \"CreatedTime\": \"2014-05-07T17:39:28.599000+00:00\",\n        \"EbsOptimized\": false,\n        \"ImageId\": \"ami-043a5034\",\n        \"InstanceMonitoring\": {\n          \"Enabled\": true\n        },\n        \"InstanceType\": \"t1.micro\",\n        \"LaunchConfigurationARN\": \"arn:aws:autoscaling:us-west-2:123456789012:launchConfiguration:98d3b196-4cf9-4e88-8ca1-8547c24ced8b:launchConfigurationName/my-launch-config\",\n        \"LaunchConfigurationName\": \"my-launch-config\",\n        \"SecurityGroups\": [\n          \"sg-67ef0308\"\n        ]\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-launch-configurations-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: LaunchConfigurationsType
---
