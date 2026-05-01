---
description: The channel through which Config delivers notifications and updated configuration states.
layout: schema
name: DeliveryChannel
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: s3BucketName
  type: object
- description: ''
  name: s3KeyPrefix
  type: object
- description: ''
  name: s3KmsKeyArn
  type: object
- description: ''
  name: snsTopicARN
  type: object
- description: ''
  name: configSnapshotDeliveryProperties
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-delivery-channel-schema.json
slug: config-delivery-channel
source_filename: config-delivery-channel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delivery-channel-schema.json\",\n  \"title\": \"DeliveryChannel\",\n  \"description\": \"The channel through which Config delivers notifications and updated configuration states.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelName\"\n        },\n        {\n          \"description\": \"The name of the delivery channel. By default, Config assigns the name \\\"default\\\" when creating the delivery channel. To change the delivery channel name, you must use the DeleteDeliveryChannel action to delete your current delivery channel, and then you must use the PutDeliveryChannel command to create a delivery channel that has the desired name.\"\n        }\n      ]\n    },\n    \"s3BucketName\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The name of the Amazon S3 bucket to which Config delivers configuration snapshots and configuration history files.</p> <p>If you specify a bucket that belongs to another Amazon Web Services account, that bucket must have policies that grant access permissions to Config. For more information, see <a href=\\\"https://docs.aws.amazon.com/config/latest/developerguide/s3-bucket-policy.html\\\">Permissions for the Amazon S3 Bucket</a> in the <i>Config Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"s3KeyPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The prefix for the specified Amazon S3 bucket.\"\n        }\n      ]\n    },\n    \"s3KmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n\
  \          \"description\": \"The Amazon Resource Name (ARN) of the Key Management Service (KMS ) KMS key (KMS key) used to encrypt objects delivered by Config. Must belong to the same Region as the destination S3 bucket.\"\n        }\n      ]\n    },\n    \"snsTopicARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the Amazon SNS topic to which Config sends notifications about configuration changes.</p> <p>If you choose a topic from another account, the topic must have policies that grant access permissions to Config. For more information, see <a href=\\\"https://docs.aws.amazon.com/config/latest/developerguide/sns-topic-policy.html\\\">Permissions for the Amazon SNS Topic</a> in the <i>Config Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"configSnapshotDeliveryProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigSnapshotDeliveryProperties\"\
  \n        },\n        {\n          \"description\": \"The options for how often Config delivers configuration snapshots to the Amazon S3 bucket.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delivery-channel-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: DeliveryChannel
---
