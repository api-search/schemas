---
description: Describes an EC2 instance.
layout: schema
name: Instance
properties_list:
- description: ''
  name: InstanceId
  type: object
- description: ''
  name: InstanceType
  type: object
- description: ''
  name: AvailabilityZone
  type: object
- description: ''
  name: LifecycleState
  type: object
- description: ''
  name: HealthStatus
  type: object
- description: ''
  name: LaunchConfigurationName
  type: object
- description: ''
  name: LaunchTemplate
  type: object
- description: ''
  name: ProtectedFromScaleIn
  type: object
- description: ''
  name: WeightedCapacity
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-instance-schema.json
slug: ec2-auto-scaling-instance
source_filename: ec2-auto-scaling-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-instance-schema.json\",\n  \"title\": \"Instance\",\n  \"description\": \"Describes an EC2 instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen19\"\n        },\n        {\n          \"description\": \"The ID of the instance.\"\n        }\n      ]\n    },\n    \"InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The instance type of the EC2 instance.\"\n        }\n      ]\n    },\n    \"AvailabilityZone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\"\
  : \"The Availability Zone in which the instance is running.\"\n        }\n      ]\n    },\n    \"LifecycleState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleState\"\n        },\n        {\n          \"description\": \"A description of the current lifecycle state. The <code>Quarantined</code> state is not used. For information about lifecycle states, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/AutoScalingGroupLifecycle.html\\\">Instance lifecycle</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>. \"\n        }\n      ]\n    },\n    \"HealthStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen32\"\n        },\n        {\n          \"description\": \"The last reported health status of the instance. <code>Healthy</code> means that the instance is healthy and should remain in service. <code>Unhealthy</code> means that the instance is unhealthy and that Amazon EC2 Auto Scaling\
  \ should terminate and replace it.\"\n        }\n      ]\n    },\n    \"LaunchConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The launch configuration associated with the instance.\"\n        }\n      ]\n    },\n    \"LaunchTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchTemplateSpecification\"\n        },\n        {\n          \"description\": \"The launch template for the instance.\"\n        }\n      ]\n    },\n    \"ProtectedFromScaleIn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceProtected\"\n        },\n        {\n          \"description\": \"Indicates whether the instance is protected from termination by Amazon EC2 Auto Scaling when scaling in.\"\n        }\n      ]\n    },\n    \"WeightedCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen32\"\
  \n        },\n        {\n          \"description\": \"<p>The number of capacity units contributed by the instance based on its instance type.</p> <p>Valid Range: Minimum value of 1. Maximum value of 999.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InstanceId\",\n    \"AvailabilityZone\",\n    \"LifecycleState\",\n    \"HealthStatus\",\n    \"ProtectedFromScaleIn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-instance-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: Instance
---
