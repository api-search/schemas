---
description: Volume schema from Amazon EBS Amazon Elastic Block Store (EBS) API
layout: schema
name: Volume
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
- description: The Amazon Resource Name (ARN) of the KMS key.
  name: kmsKeyId
  type: string
- description: The number of I/O operations per second.
  name: iops
  type: integer
- description: The throughput that the volume supports, in MiB/s.
  name: throughput
  type: integer
- description: The snapshot from which the volume was created.
  name: snapshotId
  type: string
- description: Information about the volume attachments.
  name: attachments
  type: array
- description: Any tags assigned to the volume.
  name: tags
  type: array
provider_name: Amazon EBS
provider_slug: amazon-ebs
schema_file: json-schema/ebs-openapi-volume-schema.json
slug: ebs-openapi-volume
source_filename: ebs-openapi-volume-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ebs/refs/heads/main/json-schema/ebs-openapi-volume-schema.json\",\n  \"title\": \"Volume\",\n  \"description\": \"Volume schema from Amazon EBS Amazon Elastic Block Store (EBS) API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"volumeId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the volume.\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the volume, in GiBs.\"\n    },\n    \"volumeType\": {\n      \"type\": \"string\",\n      \"description\": \"The volume type.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"creating\",\n        \"available\",\n        \"in-use\",\n        \"deleting\",\n        \"deleted\",\n        \"error\"\n      ],\n      \"description\": \"The volume state.\"\n    },\n    \"availabilityZone\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The Availability Zone for the volume.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time stamp when volume creation was initiated.\"\n    },\n    \"encrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the volume is encrypted.\"\n    },\n    \"kmsKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the KMS key.\"\n    },\n    \"iops\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of I/O operations per second.\"\n    },\n    \"throughput\": {\n      \"type\": \"integer\",\n      \"description\": \"The throughput that the volume supports, in MiB/s.\"\n    },\n    \"snapshotId\": {\n      \"type\": \"string\",\n      \"description\": \"The snapshot from which the volume was created.\"\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"\
  items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"volumeId\": {\n            \"type\": \"string\"\n          },\n          \"instanceId\": {\n            \"type\": \"string\"\n          },\n          \"device\": {\n            \"type\": \"string\"\n          },\n          \"state\": {\n            \"type\": \"string\"\n          },\n          \"attachTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n        }\n      },\n      \"description\": \"Information about the volume attachments.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"description\": \"Any tags assigned to the volume.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ebs/refs/heads/main/json-schema/ebs-openapi-volume-schema.json
tags:
- Amazon Web Services
- Block Storage
- EBS
- EC2
- Snapshots
- Storage
- Volumes
title: Volume
---
