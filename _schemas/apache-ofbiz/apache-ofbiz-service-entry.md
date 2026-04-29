---
description: A single exported OFBiz service with its metadata and invocation link.
layout: schema
name: ServiceEntry
properties_list:
- description: The service name.
  name: name
  type: string
- description: Human-readable description of the service.
  name: description
  type: string
- description: Hypermedia link to a service endpoint.
  name: link
  type: object
provider_name: Apache OFBiz
provider_slug: apache-ofbiz
schema_file: json-schema/apache-ofbiz-service-entry-schema.json
slug: apache-ofbiz-service-entry
source_filename: apache-ofbiz-service-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/json-schema/apache-ofbiz-service-entry-schema.json\",\n  \"title\": \"ServiceEntry\",\n  \"description\": \"A single exported OFBiz service with its metadata and invocation link.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The service name.\",\n      \"example\": \"findProductById\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the service.\",\n      \"example\": \"Finds productId(s) corresponding to a product reference.\"\n    },\n    \"link\": {\n      \"type\": \"object\",\n      \"description\": \"Hypermedia link to a service endpoint.\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\"\
  : \"URL to invoke the service.\",\n          \"example\": \"https://localhost:8443/rest/services/findProductById\"\n        },\n        \"rel\": {\n          \"type\": \"string\",\n          \"description\": \"Relationship type.\",\n          \"example\": \"self\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP method for accessing the service.\",\n          \"example\": \"get\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/json-schema/apache-ofbiz-service-entry-schema.json
tags:
- ERP
- CRM
- E-Commerce
- Business Applications
- Apache
- Java
- Open Source
- Supply Chain
title: ServiceEntry
---
