---
description: ListLedgersResponse schema from Amazon QLDB API
layout: schema
name: ListLedgersResponse
properties_list:
- description: ''
  name: Ledgers
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-list-ledgers-response-schema.json
slug: amazon-qldb-list-ledgers-response
source_filename: amazon-qldb-list-ledgers-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-list-ledgers-response-schema.json\",\n  \"title\": \"ListLedgersResponse\",\n  \"description\": \"ListLedgersResponse schema from Amazon QLDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Ledgers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LedgerList\"\n        },\n        {\n          \"description\": \"The array of ledger summaries that are associated with the current Amazon Web Services account and Region.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"<p>A pagination token, indicating whether there are more results available:</p> <ul> <li> <p>If <code>NextToken</code> is empty, then the last page of\
  \ results has been processed and there are no more results to be retrieved.</p> </li> <li> <p>If <code>NextToken</code> is <i>not</i> empty, then there are more results available. To retrieve the next page of results, use the value of <code>NextToken</code> in a subsequent <code>ListLedgers</code> call.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-list-ledgers-response-schema.json
tags:
- AWS
- Blockchain
- Database
- Ledger
title: ListLedgersResponse
---
