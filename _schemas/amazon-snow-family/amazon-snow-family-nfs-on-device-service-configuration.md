---
description: An object that represents the metadata and configuration settings for the NFS (Network File System) service on an Amazon Web Services Snow Family device.
layout: schema
name: NFSOnDeviceServiceConfiguration
properties_list:
- description: ''
  name: StorageLimit
  type: object
- description: ''
  name: StorageUnit
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-nfs-on-device-service-configuration-schema.json
slug: amazon-snow-family-nfs-on-device-service-configuration
source_filename: amazon-snow-family-nfs-on-device-service-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-nfs-on-device-service-configuration-schema.json\",\n  \"title\": \"NFSOnDeviceServiceConfiguration\",\n  \"description\": \"An object that represents the metadata and configuration settings for the NFS (Network File System) service on an Amazon Web Services Snow Family device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StorageLimit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageLimit\"\n        },\n        {\n          \"description\": \"The maximum NFS storage for one Snow Family device.\"\n        }\n      ]\n    },\n    \"StorageUnit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageUnit\"\n        },\n        {\n          \"description\": \"<p>The scale unit of the NFS storage on the device.</p>\
  \ <p>Valid values: TB.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-nfs-on-device-service-configuration-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: NFSOnDeviceServiceConfiguration
---
