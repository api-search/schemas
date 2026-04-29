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
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-outlierdetection-schema.json
slug: amazon-app-mesh-outlierdetection
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"OutlierDetection\",\n  \"description\": \"An object that represents the outlier detection for a virtual node's listener.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"baseEjectionDuration\": {},\n    \"interval\": {},\n    \"maxEjectionPercent\": {},\n    \"maxServerErrors\": {}\n  },\n  \"required\": [\n    \"baseEjectionDuration\",\n    \"interval\",\n    \"maxEjectionPercent\",\n    \"maxServerErrors\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-outlierdetection-schema.json
tags:
- AWS
- Microservices
- Networking
- Service Mesh
title: OutlierDetection
---
