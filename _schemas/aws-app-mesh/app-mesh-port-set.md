---
description: PortSet schema from AWS App Mesh
layout: schema
name: PortSet
properties_list: []
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-port-set-schema.json
slug: app-mesh-port-set
source_filename: app-mesh-port-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"integer\",\n    \"minimum\": 1,\n    \"maximum\": 65535\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-port-set-schema.json\",\n  \"title\": \"PortSet\",\n  \"description\": \"PortSet schema from AWS App Mesh\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-port-set-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: PortSet
---
