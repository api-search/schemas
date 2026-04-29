---
description: Schema describing the fields in a link reader response.
layout: schema
name: LinkSchema
properties_list:
- description: ''
  name: key_url
  type: string
- description: ''
  name: timestamp
  type: string
- description: ''
  name: score
  type: string
- description: ''
  name: anchor
  type: string
- description: ''
  name: linktype
  type: string
- description: ''
  name: url
  type: string
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-link-schema-schema.json
slug: apache-nutch-link-schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-link-schema-schema.json\",\n  \"title\": \"LinkSchema\",\n  \"description\": \"Schema describing the fields in a link reader response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key_url\": {\n      \"type\": \"string\",\n      \"example\": \"string\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"example\": \"int\"\n    },\n    \"score\": {\n      \"type\": \"string\",\n      \"example\": \"float\"\n    },\n    \"anchor\": {\n      \"type\": \"string\",\n      \"example\": \"string\"\n    },\n    \"linktype\": {\n      \"type\": \"string\",\n      \"example\": \"string\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-link-schema-schema.json
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: LinkSchema
---
