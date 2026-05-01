---
description: DiscoverInputSchemaResponse schema from Amazon Managed Service for Apache Flink API
layout: schema
name: DiscoverInputSchemaResponse
properties_list:
- description: ''
  name: InputSchema
  type: object
- description: ''
  name: ParsedInputRecords
  type: object
- description: ''
  name: ProcessedInputRecords
  type: object
- description: ''
  name: RawInputRecords
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-discover-input-schema-response-schema.json
slug: amazon-managed-apache-flink-discover-input-schema-response
source_filename: amazon-managed-apache-flink-discover-input-schema-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-discover-input-schema-response-schema.json\",\n  \"title\": \"DiscoverInputSchemaResponse\",\n  \"description\": \"DiscoverInputSchemaResponse schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputSchema\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceSchema\"\n        },\n        {\n          \"description\": \"The schema inferred from the streaming source. It identifies the format of the data in the streaming source and how each data element maps to corresponding columns in the in-application stream that you can create.\"\n        }\n      ]\n    },\n    \"ParsedInputRecords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ParsedInputRecords\"\
  \n        },\n        {\n          \"description\": \"An array of elements, where each element corresponds to a row in a stream record (a stream record can have more than one row).\"\n        }\n      ]\n    },\n    \"ProcessedInputRecords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProcessedInputRecords\"\n        },\n        {\n          \"description\": \"The stream data that was modified by the processor specified in the <code>InputProcessingConfiguration</code> parameter.\"\n        }\n      ]\n    },\n    \"RawInputRecords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RawInputRecords\"\n        },\n        {\n          \"description\": \"The raw stream data that was sampled to infer the schema.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-discover-input-schema-response-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: DiscoverInputSchemaResponse
---
