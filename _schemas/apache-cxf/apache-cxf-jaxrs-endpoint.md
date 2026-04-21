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
