---
description: GetRevisionRequest schema from Amazon QLDB API
layout: schema
name: GetRevisionRequest
properties_list:
- description: ''
  name: BlockAddress
  type: object
- description: ''
  name: DocumentId
  type: object
- description: ''
  name: DigestTipAddress
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-get-revision-request-schema.json
slug: amazon-qldb-get-revision-request
source_filename: amazon-qldb-get-revision-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-get-revision-request-schema.json\",\n  \"title\": \"GetRevisionRequest\",\n  \"description\": \"GetRevisionRequest schema from Amazon QLDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BlockAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValueHolder\"\n        },\n        {\n          \"description\": \"<p>The block location of the document revision to be verified. An address is an Amazon Ion structure that has two fields: <code>strandId</code> and <code>sequenceNo</code>.</p> <p>For example: <code>{strandId:\\\"BlFTjlSXze9BIh1KOszcE3\\\",sequenceNo:14}</code>.</p>\"\n        }\n      ]\n    },\n    \"DocumentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UniqueId\"\n        },\n        {\n          \"description\"\
  : \"The UUID (represented in Base62-encoded text) of the document to be verified.\"\n        }\n      ]\n    },\n    \"DigestTipAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValueHolder\"\n        },\n        {\n          \"description\": \"<p>The latest block location covered by the digest for which to request a proof. An address is an Amazon Ion structure that has two fields: <code>strandId</code> and <code>sequenceNo</code>.</p> <p>For example: <code>{strandId:\\\"BlFTjlSXze9BIh1KOszcE3\\\",sequenceNo:49}</code>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BlockAddress\",\n    \"DocumentId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-get-revision-request-schema.json
tags:
- Blockchain
- Database
- Ledger
title: GetRevisionRequest
---
