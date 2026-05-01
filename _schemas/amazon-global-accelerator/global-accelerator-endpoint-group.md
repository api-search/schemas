---
description: A complex type for the endpoint group. An Amazon Web Services Region can have only one endpoint group for a specific listener.
layout: schema
name: EndpointGroup
properties_list:
- description: ''
  name: EndpointGroupArn
  type: object
- description: ''
  name: EndpointGroupRegion
  type: object
- description: ''
  name: EndpointDescriptions
  type: object
- description: ''
  name: TrafficDialPercentage
  type: object
- description: ''
  name: HealthCheckPort
  type: object
- description: ''
  name: HealthCheckProtocol
  type: object
- description: ''
  name: HealthCheckPath
  type: object
- description: ''
  name: HealthCheckIntervalSeconds
  type: object
- description: ''
  name: ThresholdCount
  type: object
- description: ''
  name: PortOverrides
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-endpoint-group-schema.json
slug: global-accelerator-endpoint-group
source_filename: global-accelerator-endpoint-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-endpoint-group-schema.json\",\n  \"title\": \"EndpointGroup\",\n  \"description\": \"A complex type for the endpoint group. An Amazon Web Services Region can have only one endpoint group for a specific listener. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the endpoint group.\"\n        }\n      ]\n    },\n    \"EndpointGroupRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Region where the endpoint group is located.\"\n        }\n      ]\n\
  \    },\n    \"EndpointDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointDescriptions\"\n        },\n        {\n          \"description\": \"The list of endpoint objects.\"\n        }\n      ]\n    },\n    \"TrafficDialPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrafficDialPercentage\"\n        },\n        {\n          \"description\": \"<p>The percentage of traffic to send to an Amazon Web Services Region. Additional traffic is distributed to other endpoint groups for this listener. </p> <p>Use this action to increase (dial up) or decrease (dial down) traffic to a specific Region. The percentage is applied to the traffic that would otherwise have been routed to the Region based on optimal routing.</p> <p>The default value is 100.</p>\"\n        }\n      ]\n    },\n    \"HealthCheckPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HealthCheckPort\"\n    \
  \    },\n        {\n          \"description\": \"<p>The port that Global Accelerator uses to perform health checks on endpoints that are part of this endpoint group. </p> <p>The default port is the port for the listener that this endpoint group is associated with. If the listener port is a list, Global Accelerator uses the first specified port in the list of ports.</p>\"\n        }\n      ]\n    },\n    \"HealthCheckProtocol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HealthCheckProtocol\"\n        },\n        {\n          \"description\": \"The protocol that Global Accelerator uses to perform health checks on endpoints that are part of this endpoint group. The default value is TCP.\"\n        }\n      ]\n    },\n    \"HealthCheckPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HealthCheckPath\"\n        },\n        {\n          \"description\": \"If the protocol is HTTP/S, then this value provides the ping path that\
  \ Global Accelerator uses for the destination on the endpoints for health checks. The default is slash (/).\"\n        }\n      ]\n    },\n    \"HealthCheckIntervalSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HealthCheckIntervalSeconds\"\n        },\n        {\n          \"description\": \"The time\\u201410 seconds or 30 seconds\\u2014between health checks for each endpoint. The default value is 30.\"\n        }\n      ]\n    },\n    \"ThresholdCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThresholdCount\"\n        },\n        {\n          \"description\": \"The number of consecutive health checks required to set the state of a healthy endpoint to unhealthy, or to set an unhealthy endpoint to healthy. The default value is 3.\"\n        }\n      ]\n    },\n    \"PortOverrides\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortOverrides\"\n        },\n        {\n          \"\
  description\": \"Allows you to override the destination ports used to route traffic to an endpoint. Using a port override lets you map a list of external destination ports (that your users send traffic to) to a list of internal destination ports that you want an application endpoint to receive traffic on. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-endpoint-group-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: EndpointGroup
---
