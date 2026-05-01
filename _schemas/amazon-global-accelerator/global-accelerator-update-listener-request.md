---
description: UpdateListenerRequest schema from Amazon Global Accelerator API
layout: schema
name: UpdateListenerRequest
properties_list:
- description: ''
  name: ListenerArn
  type: object
- description: ''
  name: PortRanges
  type: object
- description: ''
  name: Protocol
  type: object
- description: ''
  name: ClientAffinity
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-update-listener-request-schema.json
slug: global-accelerator-update-listener-request
source_filename: global-accelerator-update-listener-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-listener-request-schema.json\",\n  \"title\": \"UpdateListenerRequest\",\n  \"description\": \"UpdateListenerRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ListenerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the listener to update.\"\n        }\n      ]\n    },\n    \"PortRanges\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortRanges\"\n        },\n        {\n          \"description\": \"The updated list of port ranges for the connections from clients to the accelerator.\"\n        }\n      ]\n    },\n    \"Protocol\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/Protocol\"\n        },\n        {\n          \"description\": \"The updated protocol for the connections from clients to the accelerator.\"\n        }\n      ]\n    },\n    \"ClientAffinity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientAffinity\"\n        },\n        {\n          \"description\": \"<p>Client affinity lets you direct all requests from a user to the same endpoint, if you have stateful applications, regardless of the port and protocol of the client request. Client affinity gives you control over whether to always route each client to the same specific endpoint.</p> <p>Global Accelerator uses a consistent-flow hashing algorithm to choose the optimal endpoint for a connection. If client affinity is <code>NONE</code>, Global Accelerator uses the \\\"five-tuple\\\" (5-tuple) properties\\u2014source IP address, source port, destination IP address, destination port, and protocol\\\
  u2014to select the hash value, and then chooses the best endpoint. However, with this setting, if someone uses different ports to connect to Global Accelerator, their connections might not be always routed to the same endpoint because the hash value changes. </p> <p>If you want a given client to always be routed to the same endpoint, set client affinity to <code>SOURCE_IP</code> instead. When you use the <code>SOURCE_IP</code> setting, Global Accelerator uses the \\\"two-tuple\\\" (2-tuple) properties\\u2014 source (client) IP address and destination IP address\\u2014to select the hash value.</p> <p>The default value is <code>NONE</code>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ListenerArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-listener-request-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: UpdateListenerRequest
---
