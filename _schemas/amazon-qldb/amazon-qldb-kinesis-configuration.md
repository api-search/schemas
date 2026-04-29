---
description: The configuration settings of the Amazon Kinesis Data Streams destination for an Amazon QLDB journal stream.
layout: schema
name: KinesisConfiguration
properties_list:
- description: ''
  name: StreamArn
  type: object
- description: ''
  name: AggregationEnabled
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-kinesis-configuration-schema.json
slug: amazon-qldb-kinesis-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-kinesis-configuration-schema.json\",\n  \"title\": \"KinesisConfiguration\",\n  \"description\": \"The configuration settings of the Amazon Kinesis Data Streams destination for an Amazon QLDB journal stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StreamArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Kinesis Data Streams resource.\"\n        }\n      ]\n    },\n    \"AggregationEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Enables QLDB to publish multiple data records in a single Kinesis Data Streams record, increasing the number of records sent\
  \ per API call.</p> <p> <i>This option is enabled by default.</i> Record aggregation has important implications for processing records and requires de-aggregation in your stream consumer. To learn more, see <a href=\\\"https://docs.aws.amazon.com/streams/latest/dev/kinesis-kpl-concepts.html\\\">KPL Key Concepts</a> and <a href=\\\"https://docs.aws.amazon.com/streams/latest/dev/kinesis-kpl-consumer-deaggregation.html\\\">Consumer De-aggregation</a> in the <i>Amazon Kinesis Data Streams Developer Guide</i>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"StreamArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-kinesis-configuration-schema.json
tags:
- AWS
- Blockchain
- Database
- Ledger
title: KinesisConfiguration
---
