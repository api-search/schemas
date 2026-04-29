---
description: CreateLaunchConfigurationType schema from Auto Scaling
layout: schema
name: CreateLaunchConfigurationType
properties_list:
- description: ''
  name: LaunchConfigurationName
  type: object
- description: ''
  name: ImageId
  type: object
- description: ''
  name: KeyName
  type: object
- description: ''
  name: SecurityGroups
  type: object
- description: ''
  name: ClassicLinkVPCId
  type: object
- description: ''
  name: ClassicLinkVPCSecurityGroups
  type: object
- description: ''
  name: UserData
  type: object
- description: ''
  name: InstanceId
  type: object
- description: ''
  name: InstanceType
  type: object
- description: ''
  name: KernelId
  type: object
- description: ''
  name: RamdiskId
  type: object
- description: ''
  name: BlockDeviceMappings
  type: object
- description: ''
  name: InstanceMonitoring
  type: object
- description: ''
  name: SpotPrice
  type: object
- description: ''
  name: IamInstanceProfile
  type: object
- description: ''
  name: EbsOptimized
  type: object
- description: ''
  name: AssociatePublicIpAddress
  type: object
- description: ''
  name: PlacementTenancy
  type: object
- description: ''
  name: MetadataOptions
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-create-launch-configuration-type-schema.json
slug: ec2-auto-scaling-create-launch-configuration-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-create-launch-configuration-type-schema.json\",\n  \"title\": \"CreateLaunchConfigurationType\",\n  \"description\": \"CreateLaunchConfigurationType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LaunchConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the launch configuration. This name must be unique per Region per account.\"\n        }\n      ]\n    },\n    \"ImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"<p>The ID of the Amazon Machine Image (AMI) that was assigned during registration. For more information,\
  \ see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/finding-an-ami.html\\\">Finding a Linux AMI</a> in the <i>Amazon EC2 User Guide for Linux Instances</i>.</p> <p>If you specify <code>InstanceId</code>, an <code>ImageId</code> is not required.</p>\"\n        }\n      ]\n    },\n    \"KeyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the key pair. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html\\\">Amazon EC2 key pairs and Linux instances</a> in the <i>Amazon EC2 User Guide for Linux Instances</i>.\"\n        }\n      ]\n    },\n    \"SecurityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroups\"\n        },\n        {\n          \"description\": \"A list that contains the security group IDs to assign to the instances in the Auto Scaling\
  \ group. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonVPC/latest/UserGuide/VPC_SecurityGroups.html\\\">Control traffic to resources using security groups</a> in the <i>Amazon Virtual Private Cloud User Guide</i>.\"\n        }\n      ]\n    },\n    \"ClassicLinkVPCId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"Available for backward compatibility.\"\n        }\n      ]\n    },\n    \"ClassicLinkVPCSecurityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassicLinkVPCSecurityGroups\"\n        },\n        {\n          \"description\": \"Available for backward compatibility.\"\n        }\n      ]\n    },\n    \"UserData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringUserData\"\n        },\n        {\n          \"description\": \"The user data to make available to the launched\
  \ EC2 instances. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-metadata.html\\\">Instance metadata and user data</a> (Linux) and <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/WindowsGuide/ec2-instance-metadata.html\\\">Instance metadata and user data</a> (Windows). If you are using a command line tool, base64-encoding is performed for you, and you can load the text from a file. Otherwise, you must provide base64-encoded text. User data is limited to 16 KB.\"\n        }\n      ]\n    },\n    \"InstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen19\"\n        },\n        {\n          \"description\": \"<p>The ID of the instance to use to create the launch configuration. The new launch configuration derives attributes from the instance, except for the block device mapping.</p> <p>To create a launch configuration with a block device mapping or override any other instance attributes,\
  \ specify them as part of the same request.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/create-lc-with-instanceID.html\\\">Creating a launch configuration using an EC2 instance</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"<p>Specifies the instance type of the EC2 instance. For information about available instance types, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instance-types.html#AvailableInstanceTypes\\\">Available instance types</a> in the <i>Amazon EC2 User Guide for Linux Instances</i>.</p> <p>If you specify <code>InstanceId</code>, an <code>InstanceType</code> is not required.</p>\"\n        }\n      ]\n    },\n    \"KernelId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\
  \n        },\n        {\n          \"description\": \"<p>The ID of the kernel associated with the AMI.</p> <note> <p>We recommend that you use PV-GRUB instead of kernels and RAM disks. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/UserProvidedKernels.html\\\">User provided kernels</a> in the <i>Amazon EC2 User Guide for Linux Instances</i>.</p> </note>\"\n        }\n      ]\n    },\n    \"RamdiskId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"<p>The ID of the RAM disk to select.</p> <note> <p>We recommend that you use PV-GRUB instead of kernels and RAM disks. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/UserProvidedKernels.html\\\">User provided kernels</a> in the <i>Amazon EC2 User Guide for Linux Instances</i>.</p> </note>\"\n        }\n      ]\n    },\n    \"BlockDeviceMappings\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockDeviceMappings\"\n        },\n        {\n          \"description\": \"The block device mapping entries that define the block devices to attach to the instances at launch. By default, the block devices specified in the block device mapping for the AMI are used. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/block-device-mapping-concepts.html\\\">Block device mappings</a> in the <i>Amazon EC2 User Guide for Linux Instances</i>.\"\n        }\n      ]\n    },\n    \"InstanceMonitoring\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceMonitoring\"\n        },\n        {\n          \"description\": \"<p>Controls whether instances in this group are launched with detailed (<code>true</code>) or basic (<code>false</code>) monitoring.</p> <p>The default value is <code>true</code> (enabled).</p> <important> <p>When detailed monitoring is enabled,\
  \ Amazon CloudWatch generates metrics every minute and your account is charged a fee. When you disable detailed monitoring, CloudWatch generates metrics every 5 minutes. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/latest/userguide/enable-as-instance-metrics.html\\\">Configure Monitoring for Auto Scaling Instances</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p> </important>\"\n        }\n      ]\n    },\n    \"SpotPrice\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpotPrice\"\n        },\n        {\n          \"description\": \"<p>The maximum hourly price to be paid for any Spot Instance launched to fulfill the request. Spot Instances are launched when the price you specify exceeds the current Spot price. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/launch-template-spot-instances.html\\\">Request Spot Instances for fault-tolerant and flexible applications</a> in\
  \ the <i>Amazon EC2 Auto Scaling User Guide</i>.</p> <p>Valid Range: Minimum value of 0.001</p> <note> <p>When you change your maximum price by creating a new launch configuration, running instances will continue to run as long as the maximum price for those running instances is higher than the current Spot price.</p> </note>\"\n        }\n      ]\n    },\n    \"IamInstanceProfile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen1600\"\n        },\n        {\n          \"description\": \"The name or the Amazon Resource Name (ARN) of the instance profile associated with the IAM role for the instance. The instance profile contains the IAM role. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/us-iam-role.html\\\">IAM role for applications that run on Amazon EC2 instances</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.\"\n        }\n      ]\n    },\n    \"EbsOptimized\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/EbsOptimized\"\n        },\n        {\n          \"description\": \"<p>Specifies whether the launch configuration is optimized for EBS I/O (<code>true</code>) or not (<code>false</code>). The optimization provides dedicated throughput to Amazon EBS and an optimized configuration stack to provide optimal I/O performance. This optimization is not available with all instance types. Additional fees are incurred when you enable EBS optimization for an instance type that is not EBS-optimized by default. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSOptimized.html\\\">Amazon EBS-optimized instances</a> in the <i>Amazon EC2 User Guide for Linux Instances</i>.</p> <p>The default value is <code>false</code>.</p>\"\n        }\n      ]\n    },\n    \"AssociatePublicIpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssociatePublicIpAddress\"\n        },\n   \
  \     {\n          \"description\": \"<p>Specifies whether to assign a public IPv4 address to the group's instances. If the instance is launched into a default subnet, the default is to assign a public IPv4 address, unless you disabled the option to assign a public IPv4 address on the subnet. If the instance is launched into a nondefault subnet, the default is not to assign a public IPv4 address, unless you enabled the option to assign a public IPv4 address on the subnet.</p> <p>If you specify <code>true</code>, each instance in the Auto Scaling group receives a unique public IPv4 address. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/asg-in-vpc.html\\\">Launching Auto Scaling instances in a VPC</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p> <p>If you specify this property, you must specify at least one subnet for <code>VPCZoneIdentifier</code> when you create your group.</p>\"\n        }\n      ]\n    },\n    \"PlacementTenancy\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen64\"\n        },\n        {\n          \"description\": \"<p>The tenancy of the instance, either <code>default</code> or <code>dedicated</code>. An instance with <code>dedicated</code> tenancy runs on isolated, single-tenant hardware and can only be launched into a VPC. To launch dedicated instances into a shared tenancy VPC (a VPC with the instance placement tenancy attribute set to <code>default</code>), you must set the value of this property to <code>dedicated</code>. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/auto-scaling-dedicated-instances.html\\\">Configuring instance tenancy with Amazon EC2 Auto Scaling</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p> <p>If you specify <code>PlacementTenancy</code>, you must specify at least one subnet for <code>VPCZoneIdentifier</code> when you create your group.</p> <p>Valid values: <code>default</code>\
  \ | <code>dedicated</code> </p>\"\n        }\n      ]\n    },\n    \"MetadataOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceMetadataOptions\"\n        },\n        {\n          \"description\": \"The metadata options for the instances. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/create-launch-config.html#launch-configurations-imds\\\">Configuring the Instance Metadata Options</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LaunchConfigurationName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-create-launch-configuration-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: CreateLaunchConfigurationType
---
