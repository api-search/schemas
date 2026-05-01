---
description: <p>Use this structure to let Amazon EC2 Auto Scaling do the following when the Auto Scaling group has a mixed instances policy:</p> <ul> <li> <p>Override the instance type that is specified in the launch template.</p> </li> <li> <p>Use multiple instance types.</p> </li> </ul> <p>Specify the instance types that you want, or define your instance requirements instead and let Amazon EC2 Auto Scaling provision the available instance types that meet your requirements. This can provide Amazon EC2 Auto Scaling with a larger selection of instance types to choose from when fulfilling Spot and On-Demand capacities. You can view which instance types are matched before you apply the instance requirements to your Auto Scaling group.</p> <p>After you define your instance requirements, you don't have to keep updating these settings to get new EC2 instance types automatically. Amazon EC2 Auto Scaling uses the instance requirements of the Auto Scaling group to determine whether a new EC2 instance
  type can be used.</p>
layout: schema
name: LaunchTemplateOverrides
properties_list:
- description: ''
  name: InstanceType
  type: object
- description: ''
  name: WeightedCapacity
  type: object
- description: ''
  name: LaunchTemplateSpecification
  type: object
- description: ''
  name: InstanceRequirements
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-launch-template-overrides-schema.json
slug: ec2-auto-scaling-launch-template-overrides
source_filename: ec2-auto-scaling-launch-template-overrides-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-launch-template-overrides-schema.json\",\n  \"title\": \"LaunchTemplateOverrides\",\n  \"description\": \"<p>Use this structure to let Amazon EC2 Auto Scaling do the following when the Auto Scaling group has a mixed instances policy:</p> <ul> <li> <p>Override the instance type that is specified in the launch template.</p> </li> <li> <p>Use multiple instance types.</p> </li> </ul> <p>Specify the instance types that you want, or define your instance requirements instead and let Amazon EC2 Auto Scaling provision the available instance types that meet your requirements. This can provide Amazon EC2 Auto Scaling with a larger selection of instance types to choose from when fulfilling Spot and On-Demand capacities. You can view which instance types are matched before you apply the instance\
  \ requirements to your Auto Scaling group.</p> <p>After you define your instance requirements, you don't have to keep updating these settings to get new EC2 instance types automatically. Amazon EC2 Auto Scaling uses the instance requirements of the Auto Scaling group to determine whether a new EC2 instance type can be used.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"<p>The instance type, such as <code>m3.xlarge</code>. You must specify an instance type that is supported in your requested Region and Availability Zones. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instance-types.html\\\">Instance types</a> in the <i>Amazon Elastic Compute Cloud User Guide</i>.</p> <p>You can specify up to 40 instance types per Auto Scaling group.</p>\"\n        }\n      ]\n    },\n\
  \    \"WeightedCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen32\"\n        },\n        {\n          \"description\": \"<p>If you provide a list of instance types to use, you can specify the number of capacity units provided by each instance type in terms of virtual CPUs, memory, storage, throughput, or other relative performance characteristic. When a Spot or On-Demand Instance is launched, the capacity units count toward the desired capacity. Amazon EC2 Auto Scaling launches instances until the desired capacity is totally fulfilled, even if this results in an overage. For example, if there are two units remaining to fulfill capacity, and Amazon EC2 Auto Scaling can only launch an instance with a <code>WeightedCapacity</code> of five units, the instance is launched, and the desired capacity is exceeded by three units. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/ec2-auto-scaling-mixed-instances-groups-instance-weighting.html\\\
  \">Configuring instance weighting for Amazon EC2 Auto Scaling</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>. Value must be in the range of 1\\u2013999.</p> <p>If you specify a value for <code>WeightedCapacity</code> for one instance type, you must specify a value for <code>WeightedCapacity</code> for all of them.</p> <important> <p>Every Auto Scaling group has three size parameters (<code>DesiredCapacity</code>, <code>MaxSize</code>, and <code>MinSize</code>). Usually, you set these sizes based on a specific number of instances. However, if you configure a mixed instances policy that defines weights for the instance types, you must specify these sizes with the same units that you use for weighting instances. </p> </important>\"\n        }\n      ]\n    },\n    \"LaunchTemplateSpecification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchTemplateSpecification\"\n        },\n        {\n          \"description\": \"<p>Provides a launch template\
  \ for the specified instance type or set of instance requirements. For example, some instance types might require a launch template with a different AMI. If not provided, Amazon EC2 Auto Scaling uses the launch template that's specified in the <code>LaunchTemplate</code> definition. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/ec2-auto-scaling-mixed-instances-groups-launch-template-overrides.html\\\">Specifying a different launch template for an instance type</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>. </p> <p>You can specify up to 20 launch templates per Auto Scaling group. The launch templates specified in the overrides and in the <code>LaunchTemplate</code> definition count towards this limit.</p>\"\n        }\n      ]\n    },\n    \"InstanceRequirements\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceRequirements\"\n        },\n        {\n          \"description\": \"<p>The instance requirements.\
  \ Amazon EC2 Auto Scaling uses your specified requirements to identify instance types. Then, it uses your On-Demand and Spot allocation strategies to launch instances from these instance types.</p> <p>You can specify up to four separate sets of instance requirements per Auto Scaling group. This is useful for provisioning instances from different Amazon Machine Images (AMIs) in the same Auto Scaling group. To do this, create the AMIs and create a new launch template for each AMI. Then, create a compatible set of instance requirements for each launch template. </p> <note> <p>If you specify <code>InstanceRequirements</code>, you can't specify <code>InstanceType</code>.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-launch-template-overrides-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: LaunchTemplateOverrides
---
