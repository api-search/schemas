---
description: Describes information used to set up an Amazon EBS volume specified in a block device mapping.
layout: schema
name: Ebs
properties_list:
- description: ''
  name: SnapshotId
  type: object
- description: ''
  name: VolumeSize
  type: object
- description: ''
  name: VolumeType
  type: object
- description: ''
  name: DeleteOnTermination
  type: object
- description: ''
  name: Iops
  type: object
- description: ''
  name: Encrypted
  type: object
- description: ''
  name: Throughput
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-ebs-schema.json
slug: ec2-auto-scaling-ebs
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-ebs-schema.json\",\n  \"title\": \"Ebs\",\n  \"description\": \"Describes information used to set up an Amazon EBS volume specified in a block device mapping.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SnapshotId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"<p>The snapshot ID of the volume to use.</p> <p>You must specify either a <code>VolumeSize</code> or a <code>SnapshotId</code>.</p>\"\n        }\n      ]\n    },\n    \"VolumeSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockDeviceEbsVolumeSize\"\n        },\n        {\n          \"description\": \"<p>The volume size, in GiBs. The following are the supported volumes\
  \ sizes for each volume type: </p> <ul> <li> <p> <code>gp2</code> and <code>gp3</code>: 1-16,384</p> </li> <li> <p> <code>io1</code>: 4-16,384</p> </li> <li> <p> <code>st1</code> and <code>sc1</code>: 125-16,384</p> </li> <li> <p> <code>standard</code>: 1-1,024</p> </li> </ul> <p>You must specify either a <code>SnapshotId</code> or a <code>VolumeSize</code>. If you specify both <code>SnapshotId</code> and <code>VolumeSize</code>, the volume size must be equal or greater than the size of the snapshot.</p>\"\n        }\n      ]\n    },\n    \"VolumeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockDeviceEbsVolumeType\"\n        },\n        {\n          \"description\": \"<p>The volume type. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSVolumeTypes.html\\\">Amazon EBS volume types</a> in the <i>Amazon EC2 User Guide for Linux Instances</i>.</p> <p>Valid values: <code>standard</code> | <code>io1</code> |\
  \ <code>gp2</code> | <code>st1</code> | <code>sc1</code> | <code>gp3</code> </p>\"\n        }\n      ]\n    },\n    \"DeleteOnTermination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockDeviceEbsDeleteOnTermination\"\n        },\n        {\n          \"description\": \"Indicates whether the volume is deleted on instance termination. For Amazon EC2 Auto Scaling, the default value is <code>true</code>.\"\n        }\n      ]\n    },\n    \"Iops\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockDeviceEbsIops\"\n        },\n        {\n          \"description\": \"<p>The number of input/output (I/O) operations per second (IOPS) to provision for the volume. For <code>gp3</code> and <code>io1</code> volumes, this represents the number of IOPS that are provisioned for the volume. For <code>gp2</code> volumes, this represents the baseline performance of the volume and the rate at which the volume accumulates I/O credits for\
  \ bursting. </p> <p>The following are the supported values for each volume type: </p> <ul> <li> <p> <code>gp3</code>: 3,000-16,000 IOPS</p> </li> <li> <p> <code>io1</code>: 100-64,000 IOPS</p> </li> </ul> <p>For <code>io1</code> volumes, we guarantee 64,000 IOPS only for <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instance-types.html#ec2-nitro-instances\\\">Instances built on the Nitro System</a>. Other instance families guarantee performance up to 32,000 IOPS. </p> <p> <code>Iops</code> is supported when the volume type is <code>gp3</code> or <code>io1</code> and required only when the volume type is <code>io1</code>. (Not used with <code>standard</code>, <code>gp2</code>, <code>st1</code>, or <code>sc1</code> volumes.) </p>\"\n        }\n      ]\n    },\n    \"Encrypted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockDeviceEbsEncrypted\"\n        },\n        {\n          \"description\": \"<p>Specifies whether the volume should\
  \ be encrypted. Encrypted EBS volumes can only be attached to instances that support Amazon EBS encryption. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSEncryption.html#EBSEncryption_supported_instances\\\">Supported instance types</a>. If your AMI uses encrypted volumes, you can also only launch it on supported instance types.</p> <note> <p>If you are creating a volume from a snapshot, you cannot create an unencrypted volume from an encrypted snapshot. Also, you cannot specify a KMS key ID when using a launch configuration.</p> <p>If you enable encryption by default, the EBS volumes that you create are always encrypted, either using the Amazon Web Services managed KMS key or a customer-managed KMS key, regardless of whether the snapshot was encrypted. </p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/autoscaling/ec2/userguide/ec2-auto-scaling-data-protection.html#encryption\\\">Use Amazon Web Services KMS keys to\
  \ encrypt Amazon EBS volumes</a> in the <i>Amazon EC2 Auto Scaling User Guide</i>.</p> </note>\"\n        }\n      ]\n    },\n    \"Throughput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockDeviceEbsThroughput\"\n        },\n        {\n          \"description\": \"The throughput (MiBps) to provision for a <code>gp3</code> volume.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-ebs-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: Ebs
---
