---
description: ListDomainsRequest schema from Amazon SimpleDB API
layout: schema
name: ListDomainsRequest
properties_list:
- description: ''
  name: MaxNumberOfDomains
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-list-domains-request-schema.json
slug: amazon-simpledb-list-domains-request
source_filename: amazon-simpledb-list-domains-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-list-domains-request-schema.json\",\n  \"title\": \"ListDomainsRequest\",\n  \"description\": \"ListDomainsRequest schema from Amazon SimpleDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxNumberOfDomains\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The maximum number of domain names you want returned. The range is 1 to 100. The default setting is 100.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A string informing Amazon SimpleDB where to start the next list of domain names.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-list-domains-request-schema.json
tags:
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: ListDomainsRequest
---
