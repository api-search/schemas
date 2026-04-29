---
description: Contains information about how a source CSV data file should be analyzed.
layout: schema
name: CsvFormatDescriptor
properties_list:
- description: ''
  name: FileCompression
  type: object
- description: ''
  name: Charset
  type: object
- description: ''
  name: ContainsHeader
  type: object
- description: ''
  name: Delimiter
  type: object
- description: ''
  name: HeaderList
  type: object
- description: ''
  name: QuoteSymbol
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-csv-format-descriptor-schema.json
slug: amazon-lookout-for-metrics-csv-format-descriptor
source_filename: amazon-lookout-for-metrics-csv-format-descriptor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-csv-format-descriptor-schema.json\",\n  \"title\": \"CsvFormatDescriptor\",\n  \"description\": \"Contains information about how a source CSV data file should be analyzed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileCompression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CSVFileCompression\"\n        },\n        {\n          \"description\": \"The level of compression of the source CSV file.\"\n        }\n      ]\n    },\n    \"Charset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Charset\"\n        },\n        {\n          \"description\": \"The character set in which the source CSV file is written.\"\n        }\n      ]\n    },\n    \"ContainsHeader\": {\n      \"allOf\": [\n  \
  \      {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether or not the source CSV file contains a header.\"\n        }\n      ]\n    },\n    \"Delimiter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Delimiter\"\n        },\n        {\n          \"description\": \"The character used to delimit the source CSV file.\"\n        }\n      ]\n    },\n    \"HeaderList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HeaderList\"\n        },\n        {\n          \"description\": \"A list of the source CSV file's headers, if any.\"\n        }\n      ]\n    },\n    \"QuoteSymbol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QuoteSymbol\"\n        },\n        {\n          \"description\": \"The character used as a quote character.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-csv-format-descriptor-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: CsvFormatDescriptor
---
