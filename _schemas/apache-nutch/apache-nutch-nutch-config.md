---
description: Configuration for creating a new Nutch configuration.
layout: schema
name: NutchConfig
properties_list:
- description: The identifier for this configuration.
  name: configId
  type: string
- description: If true, overwrites an existing configuration with the same ID.
  name: force
  type: boolean
- description: Key-value pairs of Nutch configuration properties.
  name: params
  type: object
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-nutch-config-schema.json
slug: apache-nutch-nutch-config
source_filename: apache-nutch-nutch-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-nutch-config-schema.json\",\n  \"title\": \"NutchConfig\",\n  \"description\": \"Configuration for creating a new Nutch configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier for this configuration.\"\n    },\n    \"force\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, overwrites an existing configuration with the same ID.\",\n      \"default\": false\n    },\n    \"params\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value pairs of Nutch configuration properties.\"\n    }\n  },\n  \"example\": {\n    \"configId\": \"my-config\",\n    \"force\": false,\n    \"params\": {\n      \"\
  http.agent.name\": \"MyBot\",\n      \"http.robots.agents\": \"MyBot,*\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-nutch-config-schema.json
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: NutchConfig
---
