---
description: AutoScalingGroupsType schema from Auto Scaling
layout: schema
name: AutoScalingGroupsType
properties_list:
- description: ''
  name: AutoScalingGroups
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-auto-scaling-groups-type-schema.json
slug: ec2-auto-scaling-auto-scaling-groups-type
source_filename: ec2-auto-scaling-auto-scaling-groups-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-auto-scaling-groups-type-schema.json\",\n  \"title\": \"AutoScalingGroupsType\",\n  \"description\": \"AutoScalingGroupsType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroups\"\n        },\n        {\n          \"description\": \"The groups.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"A string that indicates that the response contains more items than can be returned in a single response. To receive additional items, specify this string for the <code>NextToken</code> value when requesting\
  \ the next set of items. This value is null when there are no more items to return.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AutoScalingGroups\"\n  ],\n  \"example\": {\n    \"AutoScalingGroups\": [\n      {\n        \"AutoScalingGroupARN\": \"arn:aws:autoscaling:us-west-2:123456789012:autoScalingGroup:930d940e-891e-4781-a11a-7b0acd480f03:autoScalingGroupName/my-auto-scaling-group\",\n        \"AutoScalingGroupName\": \"my-auto-scaling-group\",\n        \"AvailabilityZones\": [\n          \"us-west-2c\"\n        ],\n        \"CreatedTime\": \"2013-08-19T20:53:25.584000+00:00\",\n        \"DefaultCooldown\": 300,\n        \"DesiredCapacity\": 1,\n        \"EnabledMetrics\": [],\n        \"HealthCheckGracePeriod\": 300,\n        \"HealthCheckType\": \"EC2\",\n        \"Instances\": [\n          {\n            \"AvailabilityZone\": \"us-west-2c\",\n            \"HealthStatus\": \"Healthy\",\n            \"InstanceId\": \"i-4ba0837f\",\n            \"LaunchConfigurationName\"\
  : \"my-launch-config\",\n            \"LifecycleState\": \"InService\",\n            \"ProtectedFromScaleIn\": false\n          }\n        ],\n        \"LaunchConfigurationName\": \"my-launch-config\",\n        \"LoadBalancerNames\": [],\n        \"MaxSize\": 1,\n        \"MinSize\": 0,\n        \"NewInstancesProtectedFromScaleIn\": false,\n        \"SuspendedProcesses\": [],\n        \"Tags\": [],\n        \"TerminationPolicies\": [\n          \"Default\"\n        ],\n        \"VPCZoneIdentifier\": \"subnet-12345678\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-auto-scaling-groups-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: AutoScalingGroupsType
---
