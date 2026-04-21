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
