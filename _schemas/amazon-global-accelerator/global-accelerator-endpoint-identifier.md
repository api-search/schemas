---
description: A complex type for an endpoint. Specifies information about the endpoint to remove from the endpoint group.
layout: schema
name: EndpointIdentifier
properties_list:
- description: ''
  name: EndpointId
  type: object
- description: ''
  name: ClientIPPreservationEnabled
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-endpoint-identifier-schema.json
slug: global-accelerator-endpoint-identifier
source_filename: global-accelerator-endpoint-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-endpoint-identifier-schema.json\",\n  \"title\": \"EndpointIdentifier\",\n  \"description\": \"A complex type for an endpoint. Specifies information about the endpoint to remove from the endpoint group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"<p>An ID for the endpoint. If the endpoint is a Network Load Balancer or Application Load Balancer, this is the Amazon Resource Name (ARN) of the resource. If the endpoint is an Elastic IP address, this is the Elastic IP address allocation ID. For Amazon EC2 instances, this is the EC2 instance ID. </p> <p>An Application Load Balancer can be either internal or internet-facing.</p>\"\
  \n        }\n      ]\n    },\n    \"ClientIPPreservationEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericBoolean\"\n        },\n        {\n          \"description\": \"<p>Indicates whether client IP address preservation is enabled for an endpoint. The value is true or false. </p> <p>If the value is set to true, the client's IP address is preserved in the <code>X-Forwarded-For</code> request header as traffic travels to applications on the endpoint fronted by the accelerator.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndpointId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-endpoint-identifier-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: EndpointIdentifier
---
