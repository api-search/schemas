---
description: Defines the real-time status of a Snow device's data transfer while the device is at Amazon Web Services. This data is only available while a job has a <code>JobState</code> value of <code>InProgress</code>, for both import and export jobs.
layout: schema
name: DataTransfer
properties_list:
- description: ''
  name: BytesTransferred
  type: object
- description: ''
  name: ObjectsTransferred
  type: object
- description: ''
  name: TotalBytes
  type: object
- description: ''
  name: TotalObjects
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-data-transfer-schema.json
slug: amazon-snow-family-data-transfer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-data-transfer-schema.json\",\n  \"title\": \"DataTransfer\",\n  \"description\": \"Defines the real-time status of a Snow device's data transfer while the device is at Amazon Web Services. This data is only available while a job has a <code>JobState</code> value of <code>InProgress</code>, for both import and export jobs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BytesTransferred\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The number of bytes transferred between a Snow device and Amazon S3.\"\n        }\n      ]\n    },\n    \"ObjectsTransferred\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\"\
  : \"The number of objects transferred between a Snow device and Amazon S3.\"\n        }\n      ]\n    },\n    \"TotalBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The total bytes of data for a transfer between a Snow device and Amazon S3. This value is set to 0 (zero) until all the keys that will be transferred have been listed.\"\n        }\n      ]\n    },\n    \"TotalObjects\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The total number of objects for a transfer between a Snow device and Amazon S3. This value is set to 0 (zero) until all the keys that will be transferred have been listed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-data-transfer-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: DataTransfer
---
