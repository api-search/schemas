---
description: Schema representing an Amazon Elastic Block Store volume, which provides persistent block-level storage for use with Amazon EC2 instances.
layout: schema
name: Amazon EBS Volume
properties_list:
- description: The ID of the volume.
  name: volumeId
  type: string
- description: The size of the volume, in GiBs.
  name: size
  type: integer
- description: The volume type.
  name: volumeType
  type: string
- description: The volume state.
  name: state
  type: string
- description: The Availability Zone for the volume.
  name: availabilityZone
  type: string
- description: The time stamp when volume creation was initiated.
  name: createTime
  type: string
- description: Indicates whether the volume is encrypted.
  name: encrypted
  type: boolean
- description: The Amazon Resource Name (ARN) of the AWS KMS key that was used to protect the volume encryption key.
  name: kmsKeyId
  type: string
- description: The number of I/O operations per second (IOPS). For gp3, io1, and io2 volumes only.
  name: iops
  type: integer
- description: The throughput that the volume supports, in MiB/s. For gp3 volumes only.
  name: throughput
  type: integer
- description: The snapshot from which the volume was created, if applicable.
  name: snapshotId
  type: string
- description: Indicates whether Amazon EBS Multi-Attach is enabled. For io1 and io2 volumes only.
  name: multiAttachEnabled
  type: boolean
- description: Information about the volume attachments.
  name: attachments
  type: array
- description: Any tags assigned to the volume.
  name: tags
  type: array
provider_name: Amazon EBS
provider_slug: amazon-ebs
schema_file: json-schema/amazon-ebs-volume-schema.json
slug: amazon-ebs-volume
source_filename: amazon-ebs-volume-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.apis.io/schemas/amazon-ebs-volume.json\",\n  \"title\": \"Amazon EBS Volume\",\n  \"description\": \"Schema representing an Amazon Elastic Block Store volume, which provides persistent block-level storage for use with Amazon EC2 instances.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"availabilityZone\"\n  ],\n  \"properties\": {\n    \"volumeId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the volume.\",\n      \"pattern\": \"^vol-[a-f0-9]+$\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the volume, in GiBs.\",\n      \"minimum\": 1,\n      \"maximum\": 16384\n    },\n    \"volumeType\": {\n      \"type\": \"string\",\n      \"description\": \"The volume type.\",\n      \"enum\": [\n        \"gp2\",\n        \"gp3\",\n        \"io1\",\n        \"io2\",\n        \"st1\",\n        \"sc1\",\n        \"standard\"\
  \n      ],\n      \"default\": \"gp3\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The volume state.\",\n      \"enum\": [\n        \"creating\",\n        \"available\",\n        \"in-use\",\n        \"deleting\",\n        \"deleted\",\n        \"error\"\n      ]\n    },\n    \"availabilityZone\": {\n      \"type\": \"string\",\n      \"description\": \"The Availability Zone for the volume.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time stamp when volume creation was initiated.\"\n    },\n    \"encrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the volume is encrypted.\",\n      \"default\": false\n    },\n    \"kmsKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the AWS KMS key that was used to protect the volume encryption key.\"\n    },\n    \"iops\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"The number of I/O operations per second (IOPS). For gp3, io1, and io2 volumes only.\",\n      \"minimum\": 100,\n      \"maximum\": 256000\n    },\n    \"throughput\": {\n      \"type\": \"integer\",\n      \"description\": \"The throughput that the volume supports, in MiB/s. For gp3 volumes only.\",\n      \"minimum\": 125,\n      \"maximum\": 1000\n    },\n    \"snapshotId\": {\n      \"type\": \"string\",\n      \"description\": \"The snapshot from which the volume was created, if applicable.\",\n      \"pattern\": \"^snap-[a-f0-9]*$\"\n    },\n    \"multiAttachEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether Amazon EBS Multi-Attach is enabled. For io1 and io2 volumes only.\",\n      \"default\": false\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the volume attachments.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n        \
  \  \"volumeId\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the volume.\"\n          },\n          \"instanceId\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the instance.\",\n            \"pattern\": \"^i-[a-f0-9]+$\"\n          },\n          \"device\": {\n            \"type\": \"string\",\n            \"description\": \"The device name.\"\n          },\n          \"state\": {\n            \"type\": \"string\",\n            \"description\": \"The attachment state of the volume.\",\n            \"enum\": [\n              \"attaching\",\n              \"attached\",\n              \"detaching\",\n              \"detached\",\n              \"busy\"\n            ]\n          },\n          \"attachTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The time stamp when the attachment initiated.\"\n          },\n          \"deleteOnTermination\": {\n      \
  \      \"type\": \"boolean\",\n            \"description\": \"Indicates whether the EBS volume is deleted on instance termination.\"\n          }\n        }\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Any tags assigned to the volume.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Key\": {\n            \"type\": \"string\",\n            \"description\": \"The key of the tag.\"\n          },\n          \"Value\": {\n            \"type\": \"string\",\n            \"description\": \"The value of the tag.\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ebs/refs/heads/main/json-schema/amazon-ebs-volume-schema.json
tags:
- Amazon Web Services
- Block Storage
- EBS
- EC2
- Snapshots
- Storage
- Volumes
title: Amazon EBS Volume
---
