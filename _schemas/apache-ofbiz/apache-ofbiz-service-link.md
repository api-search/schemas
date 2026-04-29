---
description: Hypermedia link to a service endpoint.
layout: schema
name: ServiceLink
properties_list:
- description: URL to invoke the service.
  name: href
  type: string
- description: Relationship type.
  name: rel
  type: string
- description: HTTP method for accessing the service.
  name: type
  type: string
provider_name: Apache OFBiz
provider_slug: apache-ofbiz
schema_file: json-schema/apache-ofbiz-service-link-schema.json
slug: apache-ofbiz-service-link
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/json-schema/apache-ofbiz-service-link-schema.json\",\n  \"title\": \"ServiceLink\",\n  \"description\": \"Hypermedia link to a service endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to invoke the service.\",\n      \"example\": \"https://localhost:8443/rest/services/findProductById\"\n    },\n    \"rel\": {\n      \"type\": \"string\",\n      \"description\": \"Relationship type.\",\n      \"example\": \"self\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"HTTP method for accessing the service.\",\n      \"example\": \"get\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/json-schema/apache-ofbiz-service-link-schema.json
tags:
- ERP
- CRM
- E-Commerce
- Business Applications
- Apache
- Java
- Open Source
- Supply Chain
title: ServiceLink
---
