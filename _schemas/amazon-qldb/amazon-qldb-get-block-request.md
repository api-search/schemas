---
description: GetBlockRequest schema from Amazon QLDB API
layout: schema
name: GetBlockRequest
properties_list:
- description: ''
  name: BlockAddress
  type: object
- description: ''
  name: DigestTipAddress
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-get-block-request-schema.json
slug: amazon-qldb-get-block-request
source_filename: amazon-qldb-get-block-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-get-block-request-schema.json\",\n  \"title\": \"GetBlockRequest\",\n  \"description\": \"GetBlockRequest schema from Amazon QLDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BlockAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValueHolder\"\n        },\n        {\n          \"description\": \"<p>The location of the block that you want to request. An address is an Amazon Ion structure that has two fields: <code>strandId</code> and <code>sequenceNo</code>.</p> <p>For example: <code>{strandId:\\\"BlFTjlSXze9BIh1KOszcE3\\\",sequenceNo:14}</code>.</p>\"\n        }\n      ]\n    },\n    \"DigestTipAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValueHolder\"\n        },\n        {\n          \"description\"\
  : \"<p>The latest block location covered by the digest for which to request a proof. An address is an Amazon Ion structure that has two fields: <code>strandId</code> and <code>sequenceNo</code>.</p> <p>For example: <code>{strandId:\\\"BlFTjlSXze9BIh1KOszcE3\\\",sequenceNo:49}</code>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BlockAddress\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-get-block-request-schema.json
tags:
- Blockchain
- Database
- Ledger
title: GetBlockRequest
---
