---
description: A backend represents an origin server that a Fastly service routes requests to for content that is not cached at the edge. Backends define the address, port, SSL configuration, health checks, and load balancing parameters for origin connections.
layout: schema
name: Fastly Backend
properties_list:
- description: The name of the backend, used as a unique identifier within the service version.
  name: name
  type: string
- description: The hostname or IPv4 address of the backend origin server.
  name: address
  type: string
- description: The port number on the backend origin server.
  name: port
  type: integer
- description: Whether to use SSL/TLS to connect to the backend.
  name: use_ssl
  type: boolean
- description: The hostname to verify for SSL certificate validation.
  name: ssl_hostname
  type: string
- description: The hostname to use when checking the backend SSL certificate.
  name: ssl_cert_hostname
  type: string
- description: The SNI hostname to use for the backend TLS connection.
  name: ssl_sni_hostname
  type: string
- description: The data center identifier to use as a shield POP for this backend.
  name: shield
  type: string
- description: The weight assigned to this backend for load balancing purposes.
  name: weight
  type: integer
- description: Maximum duration in milliseconds to wait for a connection to the backend.
  name: connect_timeout
  type: integer
- description: Maximum duration in milliseconds to wait for the first byte from the backend.
  name: first_byte_timeout
  type: integer
- description: Maximum duration in milliseconds to wait between bytes received from the backend.
  name: between_bytes_timeout
  type: integer
- description: Maximum number of simultaneous connections to the backend.
  name: max_conn
  type: integer
- description: The name of the healthcheck to use with the backend.
  name: healthcheck
  type: string
- description: Whether to auto-load-balance this backend with others that share the same healthcheck.
  name: auto_loadbalance
  type: boolean
- description: The name of a condition to apply to route requests to this backend.
  name: request_condition
  type: string
- description: A freeform descriptive note about the backend.
  name: comment
  type: string
provider_name: fastly
provider_slug: fastly
schema_file: json-schema/fastly-backend-schema.json
slug: fastly-backend
source_filename: fastly-backend-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/fastly/backend.json\",\n  \"title\": \"Fastly Backend\",\n  \"description\": \"A backend represents an origin server that a Fastly service routes requests to for content that is not cached at the edge. Backends define the address, port, SSL configuration, health checks, and load balancing parameters for origin connections.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"address\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the backend, used as a unique identifier within the service version.\",\n      \"minLength\": 1\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname or IPv4 address of the backend origin server.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port number on the backend origin server.\",\n\
  \      \"minimum\": 1,\n      \"maximum\": 65535,\n      \"default\": 80\n    },\n    \"use_ssl\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use SSL/TLS to connect to the backend.\"\n    },\n    \"ssl_hostname\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname to verify for SSL certificate validation.\"\n    },\n    \"ssl_cert_hostname\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname to use when checking the backend SSL certificate.\"\n    },\n    \"ssl_sni_hostname\": {\n      \"type\": \"string\",\n      \"description\": \"The SNI hostname to use for the backend TLS connection.\"\n    },\n    \"shield\": {\n      \"type\": \"string\",\n      \"description\": \"The data center identifier to use as a shield POP for this backend.\"\n    },\n    \"weight\": {\n      \"type\": \"integer\",\n      \"description\": \"The weight assigned to this backend for load balancing purposes.\",\n      \"minimum\": 1,\n      \"maximum\"\
  : 100\n    },\n    \"connect_timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum duration in milliseconds to wait for a connection to the backend.\",\n      \"minimum\": 0\n    },\n    \"first_byte_timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum duration in milliseconds to wait for the first byte from the backend.\",\n      \"minimum\": 0\n    },\n    \"between_bytes_timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum duration in milliseconds to wait between bytes received from the backend.\",\n      \"minimum\": 0\n    },\n    \"max_conn\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of simultaneous connections to the backend.\",\n      \"minimum\": 0\n    },\n    \"healthcheck\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the healthcheck to use with the backend.\"\n    },\n    \"auto_loadbalance\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether to auto-load-balance this backend with others that share the same healthcheck.\"\n    },\n    \"request_condition\": {\n      \"type\": \"string\",\n      \"description\": \"The name of a condition to apply to route requests to this backend.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"A freeform descriptive note about the backend.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fastly/refs/heads/main/json-schema/fastly-backend-schema.json
tags: []
title: Fastly Backend
---
