---
description: Properties of an inferred CSV format.
layout: schema
name: DetectedCsvFormatDescriptor
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
schema_file: json-schema/amazon-lookout-for-metrics-detected-csv-format-descriptor-schema.json
slug: amazon-lookout-for-metrics-detected-csv-format-descriptor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detected-csv-format-descriptor-schema.json\",\n  \"title\": \"DetectedCsvFormatDescriptor\",\n  \"description\": \"Properties of an inferred CSV format.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileCompression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectedField\"\n        },\n        {\n          \"description\": \"The format's file compression.\"\n        }\n      ]\n    },\n    \"Charset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectedField\"\n        },\n        {\n          \"description\": \"The format's charset.\"\n        }\n      ]\n    },\n    \"ContainsHeader\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectedField\"\n    \
  \    },\n        {\n          \"description\": \"Whether the format includes a header.\"\n        }\n      ]\n    },\n    \"Delimiter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectedField\"\n        },\n        {\n          \"description\": \"The format's delimiter.\"\n        }\n      ]\n    },\n    \"HeaderList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectedField\"\n        },\n        {\n          \"description\": \"The format's header list.\"\n        }\n      ]\n    },\n    \"QuoteSymbol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectedField\"\n        },\n        {\n          \"description\": \"The format's quote symbol.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detected-csv-format-descriptor-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DetectedCsvFormatDescriptor
---
