---
description: Configuration for a JAX-WS (SOAP) endpoint in Apache CXF.
layout: schema
name: JaxWsEndpoint
properties_list:
- description: WSDL publish address for the JAX-WS endpoint.
  name: address
  type: string
- description: Fully qualified Java class name of the JAX-WS service implementation.
  name: implementor
  type: string
- description: Location of the WSDL file for contract-first services.
  name: wsdlLocation
  type: string
- description: Qualified service name from the WSDL.
  name: serviceName
  type: string
- description: Qualified port/endpoint name from the WSDL.
  name: endpointName
  type: string
- description: Inbound interceptor class names.
  name: inInterceptors
  type: array
- description: Outbound interceptor class names.
  name: outInterceptors
  type: array
provider_name: Apache CXF
provider_slug: apache-cxf
schema_file: json-schema/apache-cxf-jaxws-endpoint-schema.json
slug: apache-cxf-jaxws-endpoint
source_filename: apache-cxf-jaxws-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-cxf/refs/heads/main/json-schema/apache-cxf-jaxws-endpoint-schema.json\",\n  \"title\": \"JaxWsEndpoint\",\n  \"description\": \"Configuration for a JAX-WS (SOAP) endpoint in Apache CXF.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"WSDL publish address for the JAX-WS endpoint.\",\n      \"example\": \"http://localhost:8080/HelloService\"\n    },\n    \"implementor\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified Java class name of the JAX-WS service implementation.\",\n      \"example\": \"com.example.HelloServiceImpl\"\n    },\n    \"wsdlLocation\": {\n      \"type\": \"string\",\n      \"description\": \"Location of the WSDL file for contract-first services.\",\n      \"example\": \"classpath:wsdl/hello.wsdl\"\n    },\n    \"serviceName\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Qualified service name from the WSDL.\",\n      \"example\": \"{http://example.com}HelloService\"\n    },\n    \"endpointName\": {\n      \"type\": \"string\",\n      \"description\": \"Qualified port/endpoint name from the WSDL.\",\n      \"example\": \"{http://example.com}HelloPort\"\n    },\n    \"inInterceptors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Inbound interceptor class names.\",\n      \"example\": [\n        \"org.apache.cxf.ws.security.wss4j.WSS4JInInterceptor\"\n      ]\n    },\n    \"outInterceptors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Outbound interceptor class names.\",\n      \"example\": [\n        \"org.apache.cxf.ws.security.wss4j.WSS4JOutInterceptor\"\n      ]\n    }\n  },\n  \"required\": [\n    \"address\",\n    \"implementor\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-cxf/refs/heads/main/json-schema/apache-cxf-jaxws-endpoint-schema.json
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
title: JaxWsEndpoint
---
