---
description: An object that represents the outlier detection for a virtual node's listener.
layout: schema
name: OutlierDetection
properties_list:
- description: ''
  name: baseEjectionDuration
  type: object
- description: ''
  name: interval
  type: object
- description: ''
  name: maxEjectionPercent
  type: object
- description: ''
  name: maxServerErrors
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-outlier-detection-schema.json
slug: app-mesh-outlier-detection
source_filename: app-mesh-outlier-detection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"baseEjectionDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Duration\"\n        },\n        {\n          \"description\": \"The base amount of time for which a host is ejected.\"\n        }\n      ]\n    },\n    \"interval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Duration\"\n        },\n        {\n          \"description\": \"The time interval between ejection sweep analysis.\"\n        }\n      ]\n    },\n    \"maxEjectionPercent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutlierDetectionMaxEjectionPercent\"\n        },\n        {\n          \"description\": \"Maximum percentage of hosts in load balancing pool for upstream service that can be ejected. Will eject at least one host regardless of the value.\"\n        }\n      ]\n    },\n    \"maxServerErrors\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/OutlierDetectionMaxServerErrors\"\n        },\n        {\n          \"description\": \"Number of consecutive <code>5xx</code> errors required for ejection. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"baseEjectionDuration\",\n    \"interval\",\n    \"maxEjectionPercent\",\n    \"maxServerErrors\"\n  ],\n  \"description\": \"An object that represents the outlier detection for a virtual node's listener.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-outlier-detection-schema.json\",\n  \"title\": \"OutlierDetection\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-outlier-detection-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: OutlierDetection
---
