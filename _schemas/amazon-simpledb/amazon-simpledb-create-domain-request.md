---
description: CreateDomainRequest schema from Amazon SimpleDB API
layout: schema
name: CreateDomainRequest
properties_list:
- description: ''
  name: DomainName
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-create-domain-request-schema.json
slug: amazon-simpledb-create-domain-request
source_filename: amazon-simpledb-create-domain-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-create-domain-request-schema.json\",\n  \"title\": \"CreateDomainRequest\",\n  \"description\": \"CreateDomainRequest schema from Amazon SimpleDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the domain to create. The name can range between 3 and 255 characters and can contain the following characters: a-z, A-Z, 0-9, '_', '-', and '.'.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DomainName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-create-domain-request-schema.json
tags:
- AWS
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: CreateDomainRequest
---
