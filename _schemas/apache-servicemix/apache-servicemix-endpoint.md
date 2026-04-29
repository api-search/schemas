---
description: Web service endpoint
layout: schema
name: Endpoint
properties_list:
- description: Endpoint name
  name: name
  type: string
- description: Endpoint URL address
  name: address
  type: string
- description: Endpoint type (SOAP, REST, JMS, etc.)
  name: type
  type: string
- description: WSDL URL for SOAP endpoints
  name: wsdl
  type: string
provider_name: Apache ServiceMix
provider_slug: apache-servicemix
schema_file: json-schema/apache-servicemix-endpoint-schema.json
slug: apache-servicemix-endpoint
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-endpoint-schema.json\",\n  \"title\": \"Endpoint\",\n  \"description\": \"Web service endpoint\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Endpoint name\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Endpoint URL address\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Endpoint type (SOAP, REST, JMS, etc.)\"\n    },\n    \"wsdl\": {\n      \"type\": \"string\",\n      \"description\": \"WSDL URL for SOAP endpoints\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-servicemix/refs/heads/main/json-schema/apache-servicemix-endpoint-schema.json
tags:
- Enterprise Integration
- ESB
- Integration
- Messaging
- OSGi
- Apache
- Open Source
title: Endpoint
---
