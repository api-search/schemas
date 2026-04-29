---
description: Configuration specifying a file path for reader operations.
layout: schema
name: ReaderConfig
properties_list:
- description: The path to the sequence file, link data, or node data to read.
  name: path
  type: string
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-reader-config-schema.json
slug: apache-nutch-reader-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-reader-config-schema.json\",\n  \"title\": \"ReaderConfig\",\n  \"description\": \"Configuration specifying a file path for reader operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The path to the sequence file, link data, or node data to read.\"\n    }\n  },\n  \"required\": [\n    \"path\"\n  ],\n  \"example\": {\n    \"path\": \"crawl-01/crawldb/current/part-00000/data\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-reader-config-schema.json
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: ReaderConfig
---
