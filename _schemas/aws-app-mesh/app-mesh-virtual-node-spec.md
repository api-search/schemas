---
description: An object that represents the specification of a virtual node.
layout: schema
name: VirtualNodeSpec
properties_list:
- description: ''
  name: backendDefaults
  type: object
- description: ''
  name: backends
  type: object
- description: ''
  name: listeners
  type: object
- description: ''
  name: logging
  type: object
- description: ''
  name: serviceDiscovery
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-virtual-node-spec-schema.json
slug: app-mesh-virtual-node-spec
source_filename: app-mesh-virtual-node-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"backendDefaults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BackendDefaults\"\n        },\n        {\n          \"description\": \"A reference to an object that represents the defaults for backends.\"\n        }\n      ]\n    },\n    \"backends\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Backends\"\n        },\n        {\n          \"description\": \"The backends that the virtual node is expected to send outbound traffic to.\"\n        }\n      ]\n    },\n    \"listeners\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Listeners\"\n        },\n        {\n          \"description\": \"The listener that the virtual node is expected to receive inbound traffic from. You can specify one listener.\"\n        }\n      ]\n    },\n    \"logging\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Logging\"\
  \n        },\n        {\n          \"description\": \"The inbound and outbound access logging information for the virtual node.\"\n        }\n      ]\n    },\n    \"serviceDiscovery\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceDiscovery\"\n        },\n        {\n          \"description\": \"The service discovery information for the virtual node. If your virtual node does not expect ingress traffic, you can omit this parameter. If you specify a <code>listener</code>, then you must specify service discovery information.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"An object that represents the specification of a virtual node.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-node-spec-schema.json\",\n  \"title\": \"VirtualNodeSpec\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-virtual-node-spec-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: VirtualNodeSpec
---
