---
description: An object that represents the metadata and configuration settings for the Storage Gateway service Tape Gateway type on an Amazon Web Services Snow Family device.
layout: schema
name: TGWOnDeviceServiceConfiguration
properties_list:
- description: ''
  name: StorageLimit
  type: object
- description: ''
  name: StorageUnit
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-tgw-on-device-service-configuration-schema.json
slug: amazon-snow-family-tgw-on-device-service-configuration
source_filename: amazon-snow-family-tgw-on-device-service-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-tgw-on-device-service-configuration-schema.json\",\n  \"title\": \"TGWOnDeviceServiceConfiguration\",\n  \"description\": \"An object that represents the metadata and configuration settings for the Storage Gateway service Tape Gateway type on an Amazon Web Services Snow Family device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StorageLimit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageLimit\"\n        },\n        {\n          \"description\": \"The maximum number of virtual tapes to store on one Snow Family device. Due to physical resource limitations, this value must be set to 80 for Snowball Edge.\"\n        }\n      ]\n    },\n    \"StorageUnit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageUnit\"\
  \n        },\n        {\n          \"description\": \"The scale unit of the virtual tapes on the device.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-tgw-on-device-service-configuration-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: TGWOnDeviceServiceConfiguration
---
