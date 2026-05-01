---
description: <p>Override specific listener ports used to route traffic to endpoints that are part of an endpoint group. For example, you can create a port override in which the listener receives user traffic on ports 80 and 443, but your accelerator routes that traffic to ports 1080 and 1443, respectively, on the endpoints.</p> <p>For more information, see <a href="https://docs.aws.amazon.com/global-accelerator/latest/dg/about-endpoint-groups-port-override.html"> Overriding listener ports</a> in the <i>Global Accelerator Developer Guide</i>.</p>
layout: schema
name: PortOverride
properties_list:
- description: ''
  name: ListenerPort
  type: object
- description: ''
  name: EndpointPort
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-port-override-schema.json
slug: global-accelerator-port-override
source_filename: global-accelerator-port-override-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-port-override-schema.json\",\n  \"title\": \"PortOverride\",\n  \"description\": \"<p>Override specific listener ports used to route traffic to endpoints that are part of an endpoint group. For example, you can create a port override in which the listener receives user traffic on ports 80 and 443, but your accelerator routes that traffic to ports 1080 and 1443, respectively, on the endpoints.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/global-accelerator/latest/dg/about-endpoint-groups-port-override.html\\\"> Overriding listener ports</a> in the <i>Global Accelerator Developer Guide</i>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ListenerPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortNumber\"\
  \n        },\n        {\n          \"description\": \"The listener port that you want to map to a specific endpoint port. This is the port that user traffic arrives to the Global Accelerator on.\"\n        }\n      ]\n    },\n    \"EndpointPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortNumber\"\n        },\n        {\n          \"description\": \"The endpoint port that you want a listener port to be mapped to. This is the port on the endpoint, such as the Application Load Balancer or Amazon EC2 instance.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-port-override-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: PortOverride
---
