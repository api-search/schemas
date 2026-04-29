---
description: A child (outlink) of a fetched node.
layout: schema
name: ChildNode
properties_list:
- description: The URL of the child node.
  name: childUrl
  type: string
- description: The anchor text of the link.
  name: anchorText
  type: string
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-child-node-schema.json
slug: apache-nutch-child-node
source_filename: apache-nutch-child-node-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-child-node-schema.json\",\n  \"title\": \"ChildNode\",\n  \"description\": \"A child (outlink) of a fetched node.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"childUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the child node.\"\n    },\n    \"anchorText\": {\n      \"type\": \"string\",\n      \"description\": \"The anchor text of the link.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-child-node-schema.json
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: ChildNode
---
