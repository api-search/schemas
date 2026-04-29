---
description: ListJournalKinesisStreamsForLedgerResponse schema from Amazon QLDB API
layout: schema
name: ListJournalKinesisStreamsForLedgerResponse
properties_list:
- description: ''
  name: Streams
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-list-journal-kinesis-streams-for-ledger-response-schema.json
slug: amazon-qldb-list-journal-kinesis-streams-for-ledger-response
source_filename: amazon-qldb-list-journal-kinesis-streams-for-ledger-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-list-journal-kinesis-streams-for-ledger-response-schema.json\",\n  \"title\": \"ListJournalKinesisStreamsForLedgerResponse\",\n  \"description\": \"ListJournalKinesisStreamsForLedgerResponse schema from Amazon QLDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Streams\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JournalKinesisStreamDescriptionList\"\n        },\n        {\n          \"description\": \"The array of QLDB journal stream descriptors that are associated with the given ledger.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"<ul> <li> <p>If <code>NextToken</code> is empty, the last page of results\
  \ has been processed and there are no more results to be retrieved.</p> </li> <li> <p>If <code>NextToken</code> is <i>not</i> empty, more results are available. To retrieve the next page of results, use the value of <code>NextToken</code> in a subsequent <code>ListJournalKinesisStreamsForLedger</code> call.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-list-journal-kinesis-streams-for-ledger-response-schema.json
tags:
- AWS
- Blockchain
- Database
- Ledger
title: ListJournalKinesisStreamsForLedgerResponse
---
