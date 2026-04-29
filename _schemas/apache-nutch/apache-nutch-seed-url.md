---
description: A single seed URL entry.
layout: schema
name: SeedUrl
properties_list:
- description: The seed URL identifier.
  name: id
  type: integer
- description: The seed URL.
  name: url
  type: string
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-seed-url-schema.json
slug: apache-nutch-seed-url
source_filename: apache-nutch-seed-url-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-seed-url-schema.json\",\n  \"title\": \"SeedUrl\",\n  \"description\": \"A single seed URL entry.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"minimum\": 0,\n      \"maximum\": 9007199254740991,\n      \"description\": \"The seed URL identifier.\",\n      \"readOnly\": true\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The seed URL.\"\n    }\n  },\n  \"example\": {\n    \"url\": \"https://example.com\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-seed-url-schema.json
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: SeedUrl
---
