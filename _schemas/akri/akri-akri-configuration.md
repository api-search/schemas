---
description: Akri Configuration custom resource (configurations.akri.sh) that specifies device discovery settings and optional broker workload deployment specifications.
layout: schema
name: AkriConfiguration
properties_list:
- description: API version of the Akri Configuration resource
  name: apiVersion
  type: string
- description: Resource kind
  name: kind
  type: string
- description: Kubernetes object metadata
  name: metadata
  type: object
- description: Configuration specification
  name: spec
  type: object
provider_name: Akri
provider_slug: akri
schema_file: json-schema/akri-akri-configuration-schema.json
slug: akri-akri-configuration
source_filename: akri-akri-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akri/refs/heads/main/json-schema/akri-akri-configuration-schema.json\",\n  \"title\": \"AkriConfiguration\",\n  \"description\": \"Akri Configuration custom resource (configurations.akri.sh) that specifies device discovery settings and optional broker workload deployment specifications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"description\": \"API version of the Akri Configuration resource\",\n      \"example\": \"akri.sh/v0\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Resource kind\",\n      \"example\": \"Configuration\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Kubernetes object metadata\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"\
  Name of the configuration\",\n          \"example\": \"onvif-camera\"\n        },\n        \"namespace\": {\n          \"type\": \"string\",\n          \"description\": \"Kubernetes namespace\",\n          \"example\": \"default\"\n        }\n      }\n    },\n    \"spec\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration specification\",\n      \"properties\": {\n        \"discoveryHandler\": {\n          \"type\": \"object\",\n          \"description\": \"Discovery Handler settings for device discovery\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"Name of the Discovery Handler to use\",\n              \"example\": \"onvif\"\n            },\n            \"discoveryDetails\": {\n              \"type\": \"string\",\n              \"description\": \"Protocol-specific discovery details as a string\",\n              \"example\": \"ipAddresses:\\\\n  action: Exclude\\\\n  items:\\\\n  - 10.0.0.1\"\
  \n            },\n            \"discoveryProperties\": {\n              \"type\": \"array\",\n              \"description\": \"Additional key-value properties for Discovery Handler\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"name\": {\n                    \"type\": \"string\",\n                    \"example\": \"USERNAME_LIST\"\n                  },\n                  \"value\": {\n                    \"type\": \"string\",\n                    \"example\": \"admin\"\n                  }\n                }\n              }\n            }\n          }\n        },\n        \"capacity\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of broker replicas per device\",\n          \"example\": 1\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akri/refs/heads/main/json-schema/akri-akri-configuration-schema.json
tags:
- Device Management
- Edge Computing
- IoT
- Kubernetes
- CNCF
- Open Source
- OPC UA
- ONVIF
- udev
title: AkriConfiguration
---
