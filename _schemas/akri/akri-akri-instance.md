---
description: Akri Instance custom resource (instances.akri.sh) representing a single discovered device. Automatically created and destroyed as devices appear and disappear.
layout: schema
name: AkriInstance
properties_list:
- description: API version of the Akri Instance resource
  name: apiVersion
  type: string
- description: Resource kind
  name: kind
  type: string
- description: Kubernetes object metadata
  name: metadata
  type: object
- description: Instance specification
  name: spec
  type: object
provider_name: Akri
provider_slug: akri
schema_file: json-schema/akri-akri-instance-schema.json
slug: akri-akri-instance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akri/refs/heads/main/json-schema/akri-akri-instance-schema.json\",\n  \"title\": \"AkriInstance\",\n  \"description\": \"Akri Instance custom resource (instances.akri.sh) representing a single discovered device. Automatically created and destroyed as devices appear and disappear.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"description\": \"API version of the Akri Instance resource\",\n      \"example\": \"akri.sh/v0\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Resource kind\",\n      \"example\": \"Instance\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Kubernetes object metadata\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Instance name in\
  \ format configuration-name-hash\",\n          \"example\": \"onvif-camera-a1b2c3\"\n        },\n        \"namespace\": {\n          \"type\": \"string\",\n          \"description\": \"Kubernetes namespace\",\n          \"example\": \"default\"\n        }\n      }\n    },\n    \"spec\": {\n      \"type\": \"object\",\n      \"description\": \"Instance specification\",\n      \"properties\": {\n        \"configurationName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the parent Configuration resource\",\n          \"example\": \"onvif-camera\"\n        },\n        \"shared\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether device is shared across multiple nodes\",\n          \"example\": false\n        },\n        \"nodes\": {\n          \"type\": \"array\",\n          \"description\": \"List of nodes that can access this device\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"example\": [\n \
  \           \"node-01\",\n            \"node-02\"\n          ]\n        },\n        \"deviceUsage\": {\n          \"type\": \"object\",\n          \"description\": \"Map of slot names to broker pod names\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"metadata\": {\n          \"type\": \"object\",\n          \"description\": \"Device-specific metadata from discovery\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akri/refs/heads/main/json-schema/akri-akri-instance-schema.json
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
title: AkriInstance
---
