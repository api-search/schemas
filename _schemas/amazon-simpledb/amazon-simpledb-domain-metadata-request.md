---
description: DomainMetadataRequest schema from Amazon SimpleDB API
layout: schema
name: DomainMetadataRequest
properties_list:
- description: ''
  name: DomainName
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-domain-metadata-request-schema.json
slug: amazon-simpledb-domain-metadata-request
source_filename: amazon-simpledb-domain-metadata-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-domain-metadata-request-schema.json\",\n  \"title\": \"DomainMetadataRequest\",\n  \"description\": \"DomainMetadataRequest schema from Amazon SimpleDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the domain for which to display the metadata of.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DomainName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-domain-metadata-request-schema.json
tags:
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: DomainMetadataRequest
---
