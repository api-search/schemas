---
description: Schema describing the fields in a node reader response.
layout: schema
name: NodeSchema
properties_list:
- description: ''
  name: key_url
  type: string
- description: ''
  name: num_inlinks
  type: string
- description: ''
  name: num_outlinks
  type: string
- description: ''
  name: inlink_score
  type: string
- description: ''
  name: outlink_score
  type: string
- description: ''
  name: metadata
  type: string
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-node-schema-schema.json
slug: apache-nutch-node-schema
source_filename: apache-nutch-node-schema-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-node-schema-schema.json\",\n  \"title\": \"NodeSchema\",\n  \"description\": \"Schema describing the fields in a node reader response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key_url\": {\n      \"type\": \"string\",\n      \"example\": \"string\"\n    },\n    \"num_inlinks\": {\n      \"type\": \"string\",\n      \"example\": \"int\"\n    },\n    \"num_outlinks\": {\n      \"type\": \"string\",\n      \"example\": \"int\"\n    },\n    \"inlink_score\": {\n      \"type\": \"string\",\n      \"example\": \"float\"\n    },\n    \"outlink_score\": {\n      \"type\": \"string\",\n      \"example\": \"float\"\n    },\n    \"metadata\": {\n      \"type\": \"string\",\n      \"example\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-node-schema-schema.json
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: NodeSchema
---
