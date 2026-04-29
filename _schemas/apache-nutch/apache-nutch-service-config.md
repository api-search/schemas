---
description: Configuration for service operations such as CommonCrawl data dumps.
layout: schema
name: ServiceConfig
properties_list:
- description: The crawl identifier.
  name: crawlId
  type: string
- description: The configuration ID.
  name: confId
  type: string
- description: Additional arguments for the service operation.
  name: args
  type: object
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-service-config-schema.json
slug: apache-nutch-service-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-service-config-schema.json\",\n  \"title\": \"ServiceConfig\",\n  \"description\": \"Configuration for service operations such as CommonCrawl data dumps.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"crawlId\": {\n      \"type\": \"string\",\n      \"description\": \"The crawl identifier.\"\n    },\n    \"confId\": {\n      \"type\": \"string\",\n      \"description\": \"The configuration ID.\"\n    },\n    \"args\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Additional arguments for the service operation.\"\n    }\n  },\n  \"required\": [\n    \"crawlId\"\n  ],\n  \"example\": {\n    \"crawlId\": \"crawl-01\",\n    \"confId\": \"default\",\n    \"args\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-service-config-schema.json
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: ServiceConfig
---
