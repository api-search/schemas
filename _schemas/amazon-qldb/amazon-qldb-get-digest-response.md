---
description: GetDigestResponse schema from Amazon QLDB API
layout: schema
name: GetDigestResponse
properties_list:
- description: ''
  name: Digest
  type: object
- description: ''
  name: DigestTipAddress
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-get-digest-response-schema.json
slug: amazon-qldb-get-digest-response
source_filename: amazon-qldb-get-digest-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-get-digest-response-schema.json\",\n  \"title\": \"GetDigestResponse\",\n  \"description\": \"GetDigestResponse schema from Amazon QLDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Digest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Digest\"\n        },\n        {\n          \"description\": \"The 256-bit hash value representing the digest returned by a <code>GetDigest</code> request.\"\n        }\n      ]\n    },\n    \"DigestTipAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValueHolder\"\n        },\n        {\n          \"description\": \"The latest block location covered by the digest that you requested. An address is an Amazon Ion structure that has two fields: <code>strandId</code> and <code>sequenceNo</code>.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Digest\",\n    \"DigestTipAddress\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-get-digest-response-schema.json
tags:
- Blockchain
- Database
- Ledger
title: GetDigestResponse
---
