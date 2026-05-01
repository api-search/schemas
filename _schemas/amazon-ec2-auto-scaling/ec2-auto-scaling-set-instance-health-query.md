---
description: SetInstanceHealthQuery schema from Auto Scaling
layout: schema
name: SetInstanceHealthQuery
properties_list:
- description: ''
  name: InstanceId
  type: object
- description: ''
  name: HealthStatus
  type: object
- description: ''
  name: ShouldRespectGracePeriod
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-set-instance-health-query-schema.json
slug: ec2-auto-scaling-set-instance-health-query
source_filename: ec2-auto-scaling-set-instance-health-query-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-set-instance-health-query-schema.json\",\n  \"title\": \"SetInstanceHealthQuery\",\n  \"description\": \"SetInstanceHealthQuery schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen19\"\n        },\n        {\n          \"description\": \"The ID of the instance.\"\n        }\n      ]\n    },\n    \"HealthStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen32\"\n        },\n        {\n          \"description\": \"The health status of the instance. Set to <code>Healthy</code> to have the instance remain in service. Set to <code>Unhealthy</code> to have the instance be out of service. Amazon EC2 Auto\
  \ Scaling terminates and replaces the unhealthy instance.\"\n        }\n      ]\n    },\n    \"ShouldRespectGracePeriod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShouldRespectGracePeriod\"\n        },\n        {\n          \"description\": \"<p>If the Auto Scaling group of the specified instance has a <code>HealthCheckGracePeriod</code> specified for the group, by default, this call respects the grace period. Set this to <code>False</code>, to have the call not respect the grace period associated with the group.</p> <p>For more information about the health check grace period, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/APIReference/API_CreateAutoScalingGroup.html\\\">CreateAutoScalingGroup</a> in the <i>Amazon EC2 Auto Scaling API Reference</i>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InstanceId\",\n    \"HealthStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-set-instance-health-query-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: SetInstanceHealthQuery
---
