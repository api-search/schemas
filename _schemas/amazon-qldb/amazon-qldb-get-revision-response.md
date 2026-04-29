---
description: GetRevisionResponse schema from Amazon QLDB API
layout: schema
name: GetRevisionResponse
properties_list:
- description: ''
  name: Proof
  type: object
- description: ''
  name: Revision
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-get-revision-response-schema.json
slug: amazon-qldb-get-revision-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-get-revision-response-schema.json\",\n  \"title\": \"GetRevisionResponse\",\n  \"description\": \"GetRevisionResponse schema from Amazon QLDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Proof\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValueHolder\"\n        },\n        {\n          \"description\": \"The proof object in Amazon Ion format returned by a <code>GetRevision</code> request. A proof contains the list of hash values that are required to recalculate the specified digest using a Merkle tree, starting with the specified document revision.\"\n        }\n      ]\n    },\n    \"Revision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValueHolder\"\n        },\n        {\n          \"description\": \"The document\
  \ revision data object in Amazon Ion format.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Revision\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-get-revision-response-schema.json
tags:
- AWS
- Blockchain
- Database
- Ledger
title: GetRevisionResponse
---
