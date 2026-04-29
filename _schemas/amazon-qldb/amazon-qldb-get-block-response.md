---
description: GetBlockResponse schema from Amazon QLDB API
layout: schema
name: GetBlockResponse
properties_list:
- description: ''
  name: Block
  type: object
- description: ''
  name: Proof
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-get-block-response-schema.json
slug: amazon-qldb-get-block-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-get-block-response-schema.json\",\n  \"title\": \"GetBlockResponse\",\n  \"description\": \"GetBlockResponse schema from Amazon QLDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Block\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValueHolder\"\n        },\n        {\n          \"description\": \"The block data object in Amazon Ion format.\"\n        }\n      ]\n    },\n    \"Proof\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValueHolder\"\n        },\n        {\n          \"description\": \"The proof object in Amazon Ion format returned by a <code>GetBlock</code> request. A proof contains the list of hash values required to recalculate the specified digest using a Merkle tree, starting with the specified block.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Block\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-get-block-response-schema.json
tags:
- AWS
- Blockchain
- Database
- Ledger
title: GetBlockResponse
---
