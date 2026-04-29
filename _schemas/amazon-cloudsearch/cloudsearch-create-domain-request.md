---
description: CreateDomainRequest schema
layout: schema
name: CreateDomainRequest
properties_list:
- description: A name for the domain you are creating.
  name: DomainName
  type: string
provider_name: Amazon CloudSearch
provider_slug: amazon-cloudsearch
schema_file: json-schema/cloudsearch-create-domain-request-schema.json
slug: cloudsearch-create-domain-request
source_filename: cloudsearch-create-domain-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudsearch/refs/heads/main/json-schema/cloudsearch-create-domain-request-schema.json\",\n  \"title\": \"CreateDomainRequest\",\n  \"description\": \"CreateDomainRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainName\": {\n      \"type\": \"string\",\n      \"description\": \"A name for the domain you are creating.\",\n      \"minLength\": 3,\n      \"maxLength\": 28\n    }\n  },\n  \"required\": [\n    \"DomainName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudsearch/refs/heads/main/json-schema/cloudsearch-create-domain-request-schema.json
tags:
- AWS
- CloudSearch
- Search
- Full-Text Search
- Managed
title: CreateDomainRequest
---
