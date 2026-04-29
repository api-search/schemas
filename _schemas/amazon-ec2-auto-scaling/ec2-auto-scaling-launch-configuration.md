---
description: Describes a launch configuration.
layout: schema
name: LaunchConfiguration
properties_list:
- description: ''
  name: LaunchConfigurationName
  type: object
- description: ''
  name: LaunchConfigurationARN
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
  name: CreatedTime
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
schema_file: json-schema/ec2-auto-scaling-launch-configuration-schema.json
slug: ec2-auto-scaling-launch-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-launch-configuration-schema.json\",\n  \"title\": \"LaunchConfiguration\",\n  \"description\": \"Describes a launch configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LaunchConfigurationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the launch configuration.\"\n        }\n      ]\n    },\n    \"LaunchConfigurationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the launch configuration.\"\n        }\n      ]\n    },\n    \"ImageId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\
  \n        },\n        {\n          \"description\": \"The ID of the Amazon Machine Image (AMI) to use to launch your EC2 instances. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/finding-an-ami.html\\\">Find a Linux AMI</a> in the <i>Amazon EC2 User Guide for Linux Instances</i>.\"\n        }\n      ]\n    },\n    \"KeyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"<p>The name of the key pair.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html\\\">Amazon EC2 Key Pairs</a> in the <i>Amazon EC2 User Guide for Linux Instances</i>.</p>\"\n        }\n      ]\n    },\n    \"SecurityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroups\"\n        },\n        {\n          \"description\": \"A list that contains the security groups\
  \ to assign to the instances in the Auto Scaling group. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonVPC/latest/UserGuide/VPC_SecurityGroups.html\\\">Security Groups for Your VPC</a> in the <i>Amazon Virtual Private Cloud User Guide</i>.\"\n        }\n      ]\n    },\n    \"ClassicLinkVPCId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"Available for backward compatibility.\"\n        }\n      ]\n    },\n    \"ClassicLinkVPCSecurityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassicLinkVPCSecurityGroups\"\n        },\n        {\n          \"description\": \"Available for backward compatibility.\"\n        }\n      ]\n    },\n    \"UserData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringUserData\"\n        },\n        {\n          \"description\": \"The user data to make\
  \ available to the launched EC2 instances. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-metadata.html\\\">Instance metadata and user data</a> (Linux) and <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/WindowsGuide/ec2-instance-metadata.html\\\">Instance metadata and user data</a> (Windows). If you are using a command line tool, base64-encoding is performed for you, and you can load the text from a file. Otherwise, you must provide base64-encoded text. User data is limited to 16 KB.\"\n        }\n      ]\n    },\n    \"InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The instance type for the instances. For information about available instance types, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instance-types.html#AvailableInstanceTypes\\\">Available instance types</a> in the <i>Amazon\
  \ EC2 User Guide for Linux Instances</i>.\"\n        }\n      ]\n    },\n    \"KernelId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The ID of the kernel associated with the AMI.\"\n        }\n      ]\n    },\n    \"RamdiskId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The ID of the RAM disk associated with the AMI.\"\n        }\n      ]\n    },\n    \"BlockDeviceMappings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockDeviceMappings\"\n        },\n        {\n          \"description\": \"The block device mapping entries that define the block devices to attach to the instances at launch. By default, the block devices specified in the block device mapping for the AMI are used. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/block-device-mapping-concepts.html\\\
  \">Block Device Mapping</a> in the <i>Amazon EC2 User Guide for Linux Instances</i>.\"\n        }\n      ]\n    },\n    \"InstanceMonitoring\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceMonitoring\"\n        },\n        {\n          \"description\": \"<p>Controls whether instances in this group are launched with detailed (<code>true</code>) or basic (<code>false</code>) monitoring.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/latest/userguide/enable-as-instance-metrics.html\\\">Configure Monitoring for Auto Scaling Instances</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"SpotPrice\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpotPrice\"\n        },\n        {\n          \"description\": \"The maximum hourly price to be paid for any Spot Instance launched to fulfill the request. Spot Instances are launched when the price you\
  \ specify exceeds the current Spot price. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/asg-launch-spot-instances.html\\\">Requesting Spot Instances</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.\"\n        }\n      ]\n    },\n    \"IamInstanceProfile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen1600\"\n        },\n        {\n          \"description\": \"The name or the Amazon Resource Name (ARN) of the instance profile associated with the IAM role for the instance. The instance profile contains the IAM role. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/us-iam-role.html\\\">IAM role for applications that run on Amazon EC2 instances</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.\"\n        }\n      ]\n    },\n    \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampType\"\n        },\n\
  \        {\n          \"description\": \"The creation date and time for the launch configuration.\"\n        }\n      ]\n    },\n    \"EbsOptimized\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EbsOptimized\"\n        },\n        {\n          \"description\": \"Specifies whether the launch configuration is optimized for EBS I/O (<code>true</code>) or not (<code>false</code>). For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSOptimized.html\\\">Amazon EBS-Optimized Instances</a> in the <i>Amazon EC2 User Guide for Linux Instances</i>.\"\n        }\n      ]\n    },\n    \"AssociatePublicIpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssociatePublicIpAddress\"\n        },\n        {\n          \"description\": \"Specifies whether to assign a public IPv4 address to the group's instances. If the instance is launched into a default subnet, the default is to assign a public\
  \ IPv4 address, unless you disabled the option to assign a public IPv4 address on the subnet. If the instance is launched into a nondefault subnet, the default is not to assign a public IPv4 address, unless you enabled the option to assign a public IPv4 address on the subnet. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/asg-in-vpc.html\\\">Launching Auto Scaling instances in a VPC</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.\"\n        }\n      ]\n    },\n    \"PlacementTenancy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen64\"\n        },\n        {\n          \"description\": \"<p>The tenancy of the instance, either <code>default</code> or <code>dedicated</code>. An instance with <code>dedicated</code> tenancy runs on isolated, single-tenant hardware and can only be launched into a VPC.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/auto-scaling-dedicated-instances.html\\\
  \">Configuring instance tenancy with Amazon EC2 Auto Scaling</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"MetadataOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceMetadataOptions\"\n        },\n        {\n          \"description\": \"The metadata options for the instances. For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/create-launch-config.html#launch-configurations-imds\\\">Configuring the Instance Metadata Options</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LaunchConfigurationName\",\n    \"ImageId\",\n    \"InstanceType\",\n    \"CreatedTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-launch-configuration-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: LaunchConfiguration
---
