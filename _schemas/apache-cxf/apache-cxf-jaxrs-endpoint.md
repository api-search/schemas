---
description: Configuration for a JAX-RS (REST) endpoint in Apache CXF, including address, service class, and features.
layout: schema
name: JaxRsEndpoint
properties_list:
- description: Base URL address for the JAX-RS endpoint.
  name: address
  type: string
- description: Fully qualified Java class name of the JAX-RS service implementation.
  name: serviceClass
  type: string
- description: List of CXF feature class names to apply to this endpoint.
  name: features
  type: array
- description: JAX-RS provider class names (MessageBodyReader, MessageBodyWriter, ExceptionMapper, etc.).
  name: providers
  type: array
- description: Additional CXF endpoint properties.
  name: properties
  type: object
provider_name: Apache CXF
provider_slug: apache-cxf
schema_file: json-schema/apache-cxf-jaxrs-endpoint-schema.json
slug: apache-cxf-jaxrs-endpoint
source_filename: apache-cxf-jaxrs-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-cxf/refs/heads/main/json-schema/apache-cxf-jaxrs-endpoint-schema.json\",\n  \"title\": \"JaxRsEndpoint\",\n  \"description\": \"Configuration for a JAX-RS (REST) endpoint in Apache CXF, including address, service class, and features.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Base URL address for the JAX-RS endpoint.\",\n      \"example\": \"http://localhost:8080/api\"\n    },\n    \"serviceClass\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified Java class name of the JAX-RS service implementation.\",\n      \"example\": \"com.example.HelloServiceImpl\"\n    },\n    \"features\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of CXF feature class names to apply\
  \ to this endpoint.\",\n      \"example\": [\n        \"org.apache.cxf.ext.logging.LoggingFeature\"\n      ]\n    },\n    \"providers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"JAX-RS provider class names (MessageBodyReader, MessageBodyWriter, ExceptionMapper, etc.).\",\n      \"example\": [\n        \"com.fasterxml.jackson.jaxrs.json.JacksonJsonProvider\"\n      ]\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Additional CXF endpoint properties.\"\n    }\n  },\n  \"required\": [\n    \"address\",\n    \"serviceClass\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-cxf/refs/heads/main/json-schema/apache-cxf-jaxrs-endpoint-schema.json
tags:
- Apache
- JAX-RS
- JAX-WS
- Java
- Open Source
- REST
- SOAP
- WS-Security
- Web Services
title: JaxRsEndpoint
---
