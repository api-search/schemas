---
description: Describes a listener
layout: schema
name: Listener
properties_list:
- description: The Amazon Resource Name (ARN) of the listener
  name: listenerArn
  type: string
- description: The ARN of the load balancer
  name: loadBalancerArn
  type: string
- description: The port on which the load balancer is listening
  name: port
  type: integer
- description: The protocol for connections from clients to the load balancer
  name: protocol
  type: string
- description: The default SSL server certificate
  name: certificates
  type: array
- description: The security policy that defines supported protocols and ciphers
  name: sslPolicy
  type: string
- description: The default actions for the listener
  name: defaultActions
  type: array
provider_name: Amazon Elastic Load Balancing
provider_slug: amazon-elastic-load-balancing
schema_file: json-schema/amazon-elastic-load-balancing-listener-schema.json
slug: amazon-elastic-load-balancing-listener
source_filename: amazon-elastic-load-balancing-listener-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-listener-schema.json\",\n  \"title\": \"Listener\",\n  \"description\": \"Describes a listener\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"listenerArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the listener\"\n    },\n    \"loadBalancerArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the load balancer\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port on which the load balancer is listening\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"description\": \"The protocol for connections from clients to the load balancer\",\n      \"enum\": [\n        \"HTTP\",\n        \"HTTPS\",\n        \"TCP\",\n        \"TLS\"\
  ,\n        \"UDP\",\n        \"TCP_UDP\",\n        \"GENEVE\"\n      ]\n    },\n    \"certificates\": {\n      \"type\": \"array\",\n      \"description\": \"The default SSL server certificate\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"certificateArn\": {\n            \"type\": \"string\",\n            \"description\": \"The ARN of the certificate\"\n          }\n        }\n      }\n    },\n    \"sslPolicy\": {\n      \"type\": \"string\",\n      \"description\": \"The security policy that defines supported protocols and ciphers\"\n    },\n    \"defaultActions\": {\n      \"type\": \"array\",\n      \"description\": \"The default actions for the listener\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Action\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-listener-schema.json
tags:
- Amazon Web Services
- High Availability
- Load Balancing
- Networking
- Scalability
title: Listener
---
