---
description: Describes an Auto Scaling group.
layout: schema
name: AutoScalingGroup
properties_list:
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: AutoScalingGroupARN
  type: object
- description: ''
  name: LaunchConfigurationName
  type: object
- description: ''
  name: LaunchTemplate
  type: object
- description: ''
  name: MixedInstancesPolicy
  type: object
- description: ''
  name: MinSize
  type: object
- description: ''
  name: MaxSize
  type: object
- description: ''
  name: DesiredCapacity
  type: object
- description: ''
  name: PredictedCapacity
  type: object
- description: ''
  name: DefaultCooldown
  type: object
- description: ''
  name: AvailabilityZones
  type: object
- description: ''
  name: LoadBalancerNames
  type: object
- description: ''
  name: TargetGroupARNs
  type: object
- description: ''
  name: HealthCheckType
  type: object
- description: ''
  name: HealthCheckGracePeriod
  type: object
- description: ''
  name: Instances
  type: object
- description: ''
  name: CreatedTime
  type: object
- description: ''
  name: SuspendedProcesses
  type: object
- description: ''
  name: PlacementGroup
  type: object
- description: ''
  name: VPCZoneIdentifier
  type: object
- description: ''
  name: EnabledMetrics
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: TerminationPolicies
  type: object
- description: ''
  name: NewInstancesProtectedFromScaleIn
  type: object
- description: ''
  name: ServiceLinkedRoleARN
  type: object
- description: ''
  name: MaxInstanceLifetime
  type: object
- description: ''
  name: CapacityRebalance
  type: object
- description: ''
  name: WarmPoolConfiguration
  type: object
- description: ''
  name: WarmPoolSize
  type: object
- description: ''
  name: Context
  type: object
- description: ''
  name: DesiredCapacityType
  type: object
- description: ''
  name: DefaultInstanceWarmup
  type: object
- description: ''
  name: TrafficSources
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-auto-scaling-group-schema.json
slug: ec2-auto-scaling-auto-scaling-group
source_filename: ec2-auto-scaling-auto-scaling-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-auto-scaling-group-schema.json\",\n  \"title\": \"AutoScalingGroup\",\n  \"description\": \"Describes an Auto Scaling group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"AutoScalingGroupARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"LaunchConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\
  \n        },\n        {\n          \"description\": \"The name of the associated launch configuration.\"\n        }\n      ]\n    },\n    \"LaunchTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchTemplateSpecification\"\n        },\n        {\n          \"description\": \"The launch template for the group.\"\n        }\n      ]\n    },\n    \"MixedInstancesPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MixedInstancesPolicy\"\n        },\n        {\n          \"description\": \"The mixed instances policy for the group.\"\n        }\n      ]\n    },\n    \"MinSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupMinSize\"\n        },\n        {\n          \"description\": \"The minimum size of the group.\"\n        }\n      ]\n    },\n    \"MaxSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupMaxSize\"\n   \
  \     },\n        {\n          \"description\": \"The maximum size of the group.\"\n        }\n      ]\n    },\n    \"DesiredCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupDesiredCapacity\"\n        },\n        {\n          \"description\": \"The desired size of the group.\"\n        }\n      ]\n    },\n    \"PredictedCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupPredictedCapacity\"\n        },\n        {\n          \"description\": \"The predicted capacity of the group when it has a predictive scaling policy.\"\n        }\n      ]\n    },\n    \"DefaultCooldown\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Cooldown\"\n        },\n        {\n          \"description\": \"The duration of the default cooldown period, in seconds.\"\n        }\n      ]\n    },\n    \"AvailabilityZones\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/AvailabilityZones\"\n        },\n        {\n          \"description\": \"One or more Availability Zones for the group.\"\n        }\n      ]\n    },\n    \"LoadBalancerNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoadBalancerNames\"\n        },\n        {\n          \"description\": \"One or more load balancers associated with the group.\"\n        }\n      ]\n    },\n    \"TargetGroupARNs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetGroupARNs\"\n        },\n        {\n          \"description\": \"The Amazon Resource Names (ARN) of the target groups for your load balancer.\"\n        }\n      ]\n    },\n    \"HealthCheckType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen32\"\n        },\n        {\n          \"description\": \"A comma-separated value string of one or more health check types.\"\n        }\n      ]\n    },\n    \"HealthCheckGracePeriod\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HealthCheckGracePeriod\"\n        },\n        {\n          \"description\": \"The duration of the health check grace period, in seconds.\"\n        }\n      ]\n    },\n    \"Instances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Instances\"\n        },\n        {\n          \"description\": \"The EC2 instances associated with the group.\"\n        }\n      ]\n    },\n    \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampType\"\n        },\n        {\n          \"description\": \"The date and time the group was created.\"\n        }\n      ]\n    },\n    \"SuspendedProcesses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SuspendedProcesses\"\n        },\n        {\n          \"description\": \"The suspended processes associated with the group.\"\n        }\n      ]\n    },\n    \"PlacementGroup\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the placement group into which to launch your instances, if any.\"\n        }\n      ]\n    },\n    \"VPCZoneIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen2047\"\n        },\n        {\n          \"description\": \"One or more subnet IDs, if applicable, separated by commas.\"\n        }\n      ]\n    },\n    \"EnabledMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnabledMetrics\"\n        },\n        {\n          \"description\": \"The metrics enabled for the group.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The current state of the group when the <a>DeleteAutoScalingGroup</a>\
  \ operation is in progress.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagDescriptionList\"\n        },\n        {\n          \"description\": \"The tags for the group.\"\n        }\n      ]\n    },\n    \"TerminationPolicies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TerminationPolicies\"\n        },\n        {\n          \"description\": \"The termination policies for the group.\"\n        }\n      ]\n    },\n    \"NewInstancesProtectedFromScaleIn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceProtected\"\n        },\n        {\n          \"description\": \"Indicates whether newly launched instances are protected from termination by Amazon EC2 Auto Scaling when scaling in.\"\n        }\n      ]\n    },\n    \"ServiceLinkedRoleARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n    \
  \    },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the service-linked role that the Auto Scaling group uses to call other Amazon Web Services on your behalf.\"\n        }\n      ]\n    },\n    \"MaxInstanceLifetime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxInstanceLifetime\"\n        },\n        {\n          \"description\": \"<p>The maximum amount of time, in seconds, that an instance can be in service.</p> <p>Valid Range: Minimum value of 0.</p>\"\n        }\n      ]\n    },\n    \"CapacityRebalance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapacityRebalanceEnabled\"\n        },\n        {\n          \"description\": \"Indicates whether Capacity Rebalancing is enabled.\"\n        }\n      ]\n    },\n    \"WarmPoolConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WarmPoolConfiguration\"\n        },\n        {\n          \"description\"\
  : \"The warm pool for the group.\"\n        }\n      ]\n    },\n    \"WarmPoolSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WarmPoolSize\"\n        },\n        {\n          \"description\": \"The current size of the warm pool.\"\n        }\n      ]\n    },\n    \"Context\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Context\"\n        },\n        {\n          \"description\": \"Reserved.\"\n        }\n      ]\n    },\n    \"DesiredCapacityType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The unit of measurement for the value specified for desired capacity. Amazon EC2 Auto Scaling supports <code>DesiredCapacityType</code> for attribute-based instance type selection only.\"\n        }\n      ]\n    },\n    \"DefaultInstanceWarmup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultInstanceWarmup\"\
  \n        },\n        {\n          \"description\": \"The duration of the default instance warmup, in seconds.\"\n        }\n      ]\n    },\n    \"TrafficSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrafficSources\"\n        },\n        {\n          \"description\": \"The traffic sources associated with this Auto Scaling group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AutoScalingGroupName\",\n    \"MinSize\",\n    \"MaxSize\",\n    \"DesiredCapacity\",\n    \"DefaultCooldown\",\n    \"AvailabilityZones\",\n    \"HealthCheckType\",\n    \"CreatedTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-auto-scaling-group-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: AutoScalingGroup
---
