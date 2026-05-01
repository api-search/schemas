---
description: An object that represents the service or services on the Snow Family device that your transferred data will be exported from or imported into. Amazon Web Services Snow Family supports Amazon S3 and NFS (Network File System).
layout: schema
name: TargetOnDeviceService
properties_list:
- description: ''
  name: ServiceName
  type: object
- description: ''
  name: TransferOption
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-target-on-device-service-schema.json
slug: amazon-snow-family-target-on-device-service
source_filename: amazon-snow-family-target-on-device-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-target-on-device-service-schema.json\",\n  \"title\": \"TargetOnDeviceService\",\n  \"description\": \"An object that represents the service or services on the Snow Family device that your transferred data will be exported from or imported into. Amazon Web Services Snow Family supports Amazon S3 and NFS (Network File System).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceServiceName\"\n        },\n        {\n          \"description\": \"Specifies the name of the service on the Snow Family device that your transferred data will be exported from or imported into.\"\n        }\n      ]\n    },\n    \"TransferOption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransferOption\"\
  \n        },\n        {\n          \"description\": \"Specifies whether the data is being imported or exported. You can import or export the data, or use it locally on the device.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-target-on-device-service-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: TargetOnDeviceService
---
