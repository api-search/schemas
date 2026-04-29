---
description: FetchScanTasksRequest schema from Apache Iceberg REST Catalog API
layout: schema
name: FetchScanTasksRequest
properties_list:
- description: ''
  name: plan-task
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-fetch-scan-tasks-request-schema.json
slug: rest-catalog-open-api-fetch-scan-tasks-request
source_filename: rest-catalog-open-api-fetch-scan-tasks-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-fetch-scan-tasks-request-schema.json\",\n  \"title\": \"FetchScanTasksRequest\",\n  \"description\": \"FetchScanTasksRequest schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"plan-task\": {\n      \"$ref\": \"#/components/schemas/PlanTask\"\n    }\n  },\n  \"required\": [\n    \"plan-task\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-fetch-scan-tasks-request-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: FetchScanTasksRequest
---
