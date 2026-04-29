---
description: An object that represents a target and its relative weight. Traffic is distributed across targets according to their relative weight. For example, a weighted target with a relative weight of 50 receives five times as much traffic as one with a relative weight of 10. The total weight for all targets combined must be less than or equal to 100.
layout: schema
name: WeightedTarget
properties_list:
- description: ''
  name: port
  type: object
- description: ''
  name: virtualNode
  type: object
- description: ''
  name: weight
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-weighted-target-schema.json
slug: app-mesh-weighted-target
source_filename: app-mesh-weighted-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListenerPort\"\n        },\n        {\n          \"description\": \"The targeted port of the weighted object.\"\n        }\n      ]\n    },\n    \"virtualNode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The virtual node to associate with the weighted target.\"\n        }\n      ]\n    },\n    \"weight\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PercentInt\"\n        },\n        {\n          \"description\": \"The relative weight of the weighted target.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"virtualNode\",\n    \"weight\"\n  ],\n  \"description\": \"An object that represents a target and its relative weight. Traffic is distributed across targets according to their relative weight.\
  \ For example, a weighted target with a relative weight of 50 receives five times as much traffic as one with a relative weight of 10. The total weight for all targets combined must be less than or equal to 100.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-weighted-target-schema.json\",\n  \"title\": \"WeightedTarget\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-weighted-target-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: WeightedTarget
---
