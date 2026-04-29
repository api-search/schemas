---
description: Amazon S3 compatible storage on Snow family devices configuration items.
layout: schema
name: S3OnDeviceServiceConfiguration
properties_list:
- description: ''
  name: StorageLimit
  type: object
- description: ''
  name: StorageUnit
  type: object
- description: ''
  name: ServiceSize
  type: object
- description: ''
  name: FaultTolerance
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-s3-on-device-service-configuration-schema.json
slug: amazon-snow-family-s3-on-device-service-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-s3-on-device-service-configuration-schema.json\",\n  \"title\": \"S3OnDeviceServiceConfiguration\",\n  \"description\": \"Amazon S3 compatible storage on Snow family devices configuration items.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StorageLimit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3StorageLimit\"\n        },\n        {\n          \"description\": \"If the specified storage limit value matches storage limit of one of the defined configurations, that configuration will be used. If the specified storage limit value does not match any defined configuration, the request will fail. If more than one configuration has the same storage limit as specified, the other input need to be provided.\"\n        }\n      ]\n    },\n    \"\
  StorageUnit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageUnit\"\n        },\n        {\n          \"description\": \"Storage unit. Currently the only supported unit is TB.\"\n        }\n      ]\n    },\n    \"ServiceSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceSize\"\n        },\n        {\n          \"description\": \"Applicable when creating a cluster. Specifies how many nodes are needed for Amazon S3 compatible storage on Snow family devices. If specified, the other input can be omitted.\"\n        }\n      ]\n    },\n    \"FaultTolerance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeFaultTolerance\"\n        },\n        {\n          \"description\": \"&gt;Fault tolerance level of the cluster. This indicates the number of nodes that can go down without degrading the performance of the cluster. This additional input helps when the specified <code>StorageLimit</code>\
  \ matches more than one Amazon S3 compatible storage on Snow family devices service configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-s3-on-device-service-configuration-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: S3OnDeviceServiceConfiguration
---
