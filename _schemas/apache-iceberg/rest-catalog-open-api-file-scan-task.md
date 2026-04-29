---
description: FileScanTask schema from Apache Iceberg REST Catalog API
layout: schema
name: FileScanTask
properties_list:
- description: ''
  name: data-file
  type: object
- description: A list of indices in the delete files array (0-based)
  name: delete-file-references
  type: array
- description: An optional filter to be applied to rows in this file scan task. If the residual is not present, the client must produce the residual or use the original filter.
  name: residual-filter
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-file-scan-task-schema.json
slug: rest-catalog-open-api-file-scan-task
source_filename: rest-catalog-open-api-file-scan-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-file-scan-task-schema.json\",\n  \"title\": \"FileScanTask\",\n  \"description\": \"FileScanTask schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data-file\": {\n      \"$ref\": \"#/components/schemas/DataFile\"\n    },\n    \"delete-file-references\": {\n      \"description\": \"A list of indices in the delete files array (0-based)\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"residual-filter\": {\n      \"description\": \"An optional filter to be applied to rows in this file scan task.\\nIf the residual is not present, the client must produce the residual or use the original filter.\",\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Expression\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"data-file\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-file-scan-task-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: FileScanTask
---
