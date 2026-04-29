---
description: ListDomainsResult schema from Amazon SimpleDB API
layout: schema
name: ListDomainsResult
properties_list:
- description: ''
  name: DomainNames
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-list-domains-result-schema.json
slug: amazon-simpledb-list-domains-result
source_filename: amazon-simpledb-list-domains-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-list-domains-result-schema.json\",\n  \"title\": \"ListDomainsResult\",\n  \"description\": \"ListDomainsResult schema from Amazon SimpleDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainNameList\"\n        },\n        {\n          \"description\": \"A list of domain names that match the expression.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"An opaque token indicating that there are more domains than the specified <code>MaxNumberOfDomains</code> still available.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-list-domains-result-schema.json
tags:
- AWS
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: ListDomainsResult
---
