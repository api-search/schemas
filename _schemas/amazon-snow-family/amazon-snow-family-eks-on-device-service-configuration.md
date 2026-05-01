---
description: An object representing the metadata and configuration settings of EKS Anywhere on the Snow Family device.
layout: schema
name: EKSOnDeviceServiceConfiguration
properties_list:
- description: ''
  name: KubernetesVersion
  type: object
- description: ''
  name: EKSAnywhereVersion
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-eks-on-device-service-configuration-schema.json
slug: amazon-snow-family-eks-on-device-service-configuration
source_filename: amazon-snow-family-eks-on-device-service-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-eks-on-device-service-configuration-schema.json\",\n  \"title\": \"EKSOnDeviceServiceConfiguration\",\n  \"description\": \"An object representing the metadata and configuration settings of EKS Anywhere on the Snow Family device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"KubernetesVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Kubernetes version for EKS Anywhere on the Snow Family device.\"\n        }\n      ]\n    },\n    \"EKSAnywhereVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The version of EKS Anywhere on the Snow Family device.\"\n        }\n      ]\n \
  \   }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-eks-on-device-service-configuration-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: EKSOnDeviceServiceConfiguration
---
