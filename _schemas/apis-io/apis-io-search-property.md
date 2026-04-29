---
description: A representation of a URL
layout: schema
name: Property
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: url
  type: string
provider_name: APIs.io
provider_slug: apis-io
schema_file: json-schema/apis-io-search-property-schema.json
slug: apis-io-search-property
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-property-schema.json\",\n  \"title\": \"Property\",\n  \"description\": \"A representation of a URL\",\n  \"required\": [\n    \"type\",\n    \"url\"\n  ],\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"pattern\": \"^(Swagger)$|^(RAML)$|^(Blueprint)$|^(WADL)$|^(WSDL)$|^(TermsOfService)$|^(InterfaceLicense)$|^(StatusPage)$|^(Pricing)$|^(Forums)$|^(AlertsTwitterHandle)$|^(X-[A-Za-z0-9\\\\-]*)$\",\n      \"enum\": [\n        \"Swagger\",\n        \"RAML\",\n        \"Blueprint\",\n        \"WADL\",\n        \"WSDL\",\n        \"TersmOfService\",\n        \"InterfaceLicense\",\n        \"StatusPage\",\n        \"Pricing\",\n        \"Forums\"\n      ]\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"pattern\": \"^(http)|(https)://(.*)$\"\n    }\n  },\n  \"type\"\
  : \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/json-schema/apis-io-search-property-schema.json
tags:
- API Aggregation
- API Directory
- API Discovery
- API Indexing
- API Rating
- API Search
- APIs.json
- Search Engine
title: Property
---
