---
description: Completed server-side planning result
layout: schema
name: CompletedPlanningResult
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-completed-planning-result-schema.json
slug: rest-catalog-open-api-completed-planning-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-completed-planning-result-schema.json\",\n  \"title\": \"CompletedPlanningResult\",\n  \"description\": \"Completed server-side planning result\",\n  \"type\": \"object\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/ScanTasks\"\n    },\n    {\n      \"type\": \"object\",\n      \"required\": [\n        \"status\"\n      ],\n      \"properties\": {\n        \"status\": {\n          \"$ref\": \"#/components/schemas/PlanStatus\",\n          \"const\": \"completed\"\n        },\n        \"storage-credentials\": {\n          \"type\": \"array\",\n          \"description\": \"Storage credentials for accessing the files returned in the scan result.\\nIf the server returns storage credentials as part of the completed scan planning response, the expectation is for the client\
  \ to use these credentials to read the files returned in the FileScanTasks as part of the scan result.\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/StorageCredential\"\n          }\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-completed-planning-result-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: CompletedPlanningResult
---
