---
description: ''
layout: schema
name: PortMapping
properties_list:
- description: The port number on the container bound to the host port.
  name: containerPort
  type: integer
- description: The port number on the container instance to reserve for the container.
  name: hostPort
  type: integer
- description: The protocol used for the port mapping.
  name: protocol
  type: string
- description: The name to use for the port mapping (used with Service Connect).
  name: name
  type: string
- description: The application protocol used for the port mapping.
  name: appProtocol
  type: string
- description: The port number range on the container.
  name: containerPortRange
  type: string
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-port-mapping-schema.json
slug: amazon-ecs-port-mapping
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PortMapping\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"containerPort\": {\n      \"type\": \"integer\",\n      \"description\": \"The port number on the container bound to the host port.\"\n    },\n    \"hostPort\": {\n      \"type\": \"integer\",\n      \"description\": \"The port number on the container instance to reserve for the container.\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"description\": \"The protocol used for the port mapping.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name to use for the port mapping (used with Service Connect).\"\n    },\n    \"appProtocol\": {\n      \"type\": \"string\",\n      \"description\": \"The application protocol used for the port mapping.\"\n    },\n    \"containerPortRange\": {\n      \"type\": \"string\",\n      \"description\": \"The port number range on the container.\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-port-mapping-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: PortMapping
---
