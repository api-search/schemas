---
description: Information returned by service operations.
layout: schema
name: ServiceInfo
properties_list:
- description: List of file paths for the dump output.
  name: dumpPaths
  type: array
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-service-info-schema.json
slug: apache-nutch-service-info
source_filename: apache-nutch-service-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-service-info-schema.json\",\n  \"title\": \"ServiceInfo\",\n  \"description\": \"Information returned by service operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dumpPaths\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of file paths for the dump output.\"\n    }\n  },\n  \"required\": [\n    \"dumpPaths\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-service-info-schema.json
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: ServiceInfo
---
