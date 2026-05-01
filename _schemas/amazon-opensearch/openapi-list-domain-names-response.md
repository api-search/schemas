---
description: The result of a <code>ListDomainNames</code> operation. Contains the names of all domains owned by this account and their respective engine types.
layout: schema
name: ListDomainNamesResponse
properties_list:
- description: ''
  name: DomainNames
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-list-domain-names-response-schema.json
slug: openapi-list-domain-names-response
source_filename: openapi-list-domain-names-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-list-domain-names-response-schema.json\",\n  \"title\": \"ListDomainNamesResponse\",\n  \"description\": \"The result of a <code>ListDomainNames</code> operation. Contains the names of all domains owned by this account and their respective engine types.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainInfoList\"\n        },\n        {\n          \"description\": \"List of domain names and respective engine types.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-list-domain-names-response-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: ListDomainNamesResponse
---
