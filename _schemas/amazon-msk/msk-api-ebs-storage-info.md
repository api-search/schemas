---
description: <p>Contains information about the EBS storage volumes attached to Apache Kafka broker nodes.</p>
layout: schema
name: EBSStorageInfo
properties_list:
- description: ''
  name: ProvisionedThroughput
  type: object
- description: ''
  name: VolumeSize
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-ebs-storage-info-schema.json
slug: msk-api-ebs-storage-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-ebs-storage-info-schema.json\",\n  \"title\": \"EBSStorageInfo\",\n  \"description\": \"\\n            <p>Contains information about the EBS storage volumes attached to Apache Kafka broker nodes.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ProvisionedThroughput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProvisionedThroughput\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"provisionedThroughput\"\n          },\n          \"description\": \"\\n            <p>EBS volume provisioned throughput information.</p>\"\n        }\n      ]\n    },\n    \"VolumeSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max16384\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"\
  volumeSize\"\n          },\n          \"description\": \"\\n            <p>The size in GiB of the EBS volume for the data drive on each broker node.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-ebs-storage-info-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: EBSStorageInfo
---
