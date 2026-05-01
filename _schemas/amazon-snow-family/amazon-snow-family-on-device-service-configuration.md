---
description: An object that represents the metadata and configuration settings for services on an Amazon Web Services Snow Family device.
layout: schema
name: OnDeviceServiceConfiguration
properties_list:
- description: ''
  name: NFSOnDeviceService
  type: object
- description: ''
  name: TGWOnDeviceService
  type: object
- description: ''
  name: EKSOnDeviceService
  type: object
- description: ''
  name: S3OnDeviceService
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-on-device-service-configuration-schema.json
slug: amazon-snow-family-on-device-service-configuration
source_filename: amazon-snow-family-on-device-service-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-on-device-service-configuration-schema.json\",\n  \"title\": \"OnDeviceServiceConfiguration\",\n  \"description\": \"An object that represents the metadata and configuration settings for services on an Amazon Web Services Snow Family device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NFSOnDeviceService\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NFSOnDeviceServiceConfiguration\"\n        },\n        {\n          \"description\": \"Represents the NFS (Network File System) service on a Snow Family device.\"\n        }\n      ]\n    },\n    \"TGWOnDeviceService\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TGWOnDeviceServiceConfiguration\"\n        },\n        {\n          \"description\": \"Represents\
  \ the Storage Gateway service Tape Gateway type on a Snow Family device.\"\n        }\n      ]\n    },\n    \"EKSOnDeviceService\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EKSOnDeviceServiceConfiguration\"\n        },\n        {\n          \"description\": \"The configuration of EKS Anywhere on the Snow Family device.\"\n        }\n      ]\n    },\n    \"S3OnDeviceService\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3OnDeviceServiceConfiguration\"\n        },\n        {\n          \"description\": \"Configuration for Amazon S3 compatible storage on Snow family devices.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-on-device-service-configuration-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: OnDeviceServiceConfiguration
---
