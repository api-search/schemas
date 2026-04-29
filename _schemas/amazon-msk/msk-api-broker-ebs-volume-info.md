---
description: <p>Specifies the EBS volume upgrade information. The broker identifier must be set to the keyword ALL. This means the changes apply to all the brokers in the cluster.</p>
layout: schema
name: BrokerEBSVolumeInfo
properties_list:
- description: ''
  name: KafkaBrokerNodeId
  type: object
- description: ''
  name: ProvisionedThroughput
  type: object
- description: ''
  name: VolumeSizeGB
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-broker-ebs-volume-info-schema.json
slug: msk-api-broker-ebs-volume-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-broker-ebs-volume-info-schema.json\",\n  \"title\": \"BrokerEBSVolumeInfo\",\n  \"description\": \"\\n            <p>Specifies the EBS volume upgrade information. The broker identifier must be set to the keyword ALL. This means the changes apply to all the brokers in the cluster.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KafkaBrokerNodeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kafkaBrokerNodeId\"\n          },\n          \"description\": \"\\n            <p>The ID of the broker to update.</p>\"\n        }\n      ]\n    },\n    \"ProvisionedThroughput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProvisionedThroughput\"\n       \
  \ },\n        {\n          \"xml\": {\n            \"name\": \"provisionedThroughput\"\n          },\n          \"description\": \"\\n            <p>EBS volume provisioned throughput information.</p>\"\n        }\n      ]\n    },\n    \"VolumeSizeGB\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"volumeSizeGB\"\n          },\n          \"description\": \"\\n            <p>Size of the EBS volume to update.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"KafkaBrokerNodeId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-broker-ebs-volume-info-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BrokerEBSVolumeInfo
---
