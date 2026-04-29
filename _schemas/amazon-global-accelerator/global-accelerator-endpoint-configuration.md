---
description: A complex type for endpoints. A resource must be valid and active when you add it as an endpoint.
layout: schema
name: EndpointConfiguration
properties_list:
- description: ''
  name: EndpointId
  type: object
- description: ''
  name: Weight
  type: object
- description: ''
  name: ClientIPPreservationEnabled
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-endpoint-configuration-schema.json
slug: global-accelerator-endpoint-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-endpoint-configuration-schema.json\",\n  \"title\": \"EndpointConfiguration\",\n  \"description\": \"A complex type for endpoints. A resource must be valid and active when you add it as an endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"<p>An ID for the endpoint. If the endpoint is a Network Load Balancer or Application Load Balancer, this is the Amazon Resource Name (ARN) of the resource. If the endpoint is an Elastic IP address, this is the Elastic IP address allocation ID. For Amazon EC2 instances, this is the EC2 instance ID. A resource must be valid and active when you add it as an endpoint.</p>\
  \ <p>An Application Load Balancer can be either internal or internet-facing.</p>\"\n        }\n      ]\n    },\n    \"Weight\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointWeight\"\n        },\n        {\n          \"description\": \"The weight associated with the endpoint. When you add weights to endpoints, you configure Global Accelerator to route traffic based on proportions that you specify. For example, you might specify endpoint weights of 4, 5, 5, and 6 (sum=20). The result is that 4/20 of your traffic, on average, is routed to the first endpoint, 5/20 is routed both to the second and third endpoints, and 6/20 is routed to the last endpoint. For more information, see <a href=\\\"https://docs.aws.amazon.com/global-accelerator/latest/dg/about-endpoints-endpoint-weights.html\\\">Endpoint weights</a> in the <i>Global Accelerator Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"ClientIPPreservationEnabled\": {\n      \"allOf\": [\n  \
  \      {\n          \"$ref\": \"#/components/schemas/GenericBoolean\"\n        },\n        {\n          \"description\": \"<p>Indicates whether client IP address preservation is enabled for an endpoint. The value is true or false. The default value is true for new accelerators. </p> <p>If the value is set to true, the client's IP address is preserved in the <code>X-Forwarded-For</code> request header as traffic travels to applications on the endpoint fronted by the accelerator.</p> <p>Client IP address preservation is supported, in specific Amazon Web Services Regions, for endpoints that are Application Load Balancers and Amazon EC2 instances.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/global-accelerator/latest/dg/preserve-client-ip-address.html\\\"> Preserve client IP addresses in Global Accelerator</a> in the <i>Global Accelerator Developer Guide</i>.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-endpoint-configuration-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: EndpointConfiguration
---
