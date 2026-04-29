---
description: UpdateEndpointGroupRequest schema from Amazon Global Accelerator API
layout: schema
name: UpdateEndpointGroupRequest
properties_list:
- description: ''
  name: EndpointGroupArn
  type: object
- description: ''
  name: EndpointConfigurations
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
schema_file: json-schema/global-accelerator-update-endpoint-group-request-schema.json
slug: global-accelerator-update-endpoint-group-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-endpoint-group-request-schema.json\",\n  \"title\": \"UpdateEndpointGroupRequest\",\n  \"description\": \"UpdateEndpointGroupRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the endpoint group.\"\n        }\n      ]\n    },\n    \"EndpointConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointConfigurations\"\n        },\n        {\n          \"description\": \"The list of endpoint objects. A resource must be valid and active when you add it as an endpoint.\"\n      \
  \  }\n      ]\n    },\n    \"TrafficDialPercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrafficDialPercentage\"\n        },\n        {\n          \"description\": \"<p>The percentage of traffic to send to an Amazon Web Services Region. Additional traffic is distributed to other endpoint groups for this listener. </p> <p>Use this action to increase (dial up) or decrease (dial down) traffic to a specific Region. The percentage is applied to the traffic that would otherwise have been routed to the Region based on optimal routing.</p> <p>The default value is 100.</p>\"\n        }\n      ]\n    },\n    \"HealthCheckPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HealthCheckPort\"\n        },\n        {\n          \"description\": \"The port that Global Accelerator uses to check the health of endpoints that are part of this endpoint group. The default port is the listener port that this endpoint group is associated\
  \ with. If the listener port is a list of ports, Global Accelerator uses the first port in the list.\"\n        }\n      ]\n    },\n    \"HealthCheckProtocol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HealthCheckProtocol\"\n        },\n        {\n          \"description\": \"The protocol that Global Accelerator uses to check the health of endpoints that are part of this endpoint group. The default value is TCP.\"\n        }\n      ]\n    },\n    \"HealthCheckPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HealthCheckPath\"\n        },\n        {\n          \"description\": \"If the protocol is HTTP/S, then this specifies the path that is the destination for health check targets. The default value is slash (/).\"\n        }\n      ]\n    },\n    \"HealthCheckIntervalSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HealthCheckIntervalSeconds\"\n        },\n        {\n        \
  \  \"description\": \"The time\\u201410 seconds or 30 seconds\\u2014between each health check for an endpoint. The default value is 30.\"\n        }\n      ]\n    },\n    \"ThresholdCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThresholdCount\"\n        },\n        {\n          \"description\": \"The number of consecutive health checks required to set the state of a healthy endpoint to unhealthy, or to set an unhealthy endpoint to healthy. The default value is 3.\"\n        }\n      ]\n    },\n    \"PortOverrides\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortOverrides\"\n        },\n        {\n          \"description\": \"<p>Override specific listener ports used to route traffic to endpoints that are part of this endpoint group. For example, you can create a port override in which the listener receives user traffic on ports 80 and 443, but your accelerator routes that traffic to ports 1080 and 1443, respectively,\
  \ on the endpoints.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/global-accelerator/latest/dg/about-endpoint-groups-port-override.html\\\"> Overriding listener ports</a> in the <i>Global Accelerator Developer Guide</i>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndpointGroupArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-endpoint-group-request-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: UpdateEndpointGroupRequest
---
