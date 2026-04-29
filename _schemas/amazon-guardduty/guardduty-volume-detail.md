---
description: Contains EBS volume details.
layout: schema
name: VolumeDetail
properties_list:
- description: ''
  name: VolumeArn
  type: object
- description: ''
  name: VolumeType
  type: object
- description: ''
  name: DeviceName
  type: object
- description: ''
  name: VolumeSizeInGB
  type: object
- description: ''
  name: EncryptionType
  type: object
- description: ''
  name: SnapshotArn
  type: object
- description: ''
  name: KmsKeyArn
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-volume-detail-schema.json
slug: guardduty-volume-detail
source_filename: guardduty-volume-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-volume-detail-schema.json\",\n  \"title\": \"VolumeDetail\",\n  \"description\": \"Contains EBS volume details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VolumeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"volumeArn\"\n          },\n          \"description\": \"EBS volume Arn information.\"\n        }\n      ]\n    },\n    \"VolumeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"volumeType\"\n          },\n          \"description\": \"The EBS volume type.\"\n        }\n      ]\n    },\n    \"DeviceName\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"deviceName\"\n          },\n          \"description\": \"The device name for the EBS volume.\"\n        }\n      ]\n    },\n    \"VolumeSizeInGB\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"volumeSizeInGB\"\n          },\n          \"description\": \"EBS volume size in GB.\"\n        }\n      ]\n    },\n    \"EncryptionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"encryptionType\"\n          },\n          \"description\": \"EBS volume encryption type.\"\n        }\n      ]\n    },\n    \"SnapshotArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"snapshotArn\"\n          },\n          \"description\": \"Snapshot Arn of the EBS volume.\"\n        }\n      ]\n    },\n    \"KmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kmsKeyArn\"\n          },\n          \"description\": \"KMS key Arn used to encrypt the EBS volume.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-volume-detail-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: VolumeDetail
---
