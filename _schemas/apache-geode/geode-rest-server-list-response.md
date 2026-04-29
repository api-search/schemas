---
description: Response containing list of Geode cache servers
layout: schema
name: ServerListResponse
properties_list:
- description: List of server addresses
  name: servers
  type: array
provider_name: Apache Geode
provider_slug: apache-geode
schema_file: json-schema/geode-rest-server-list-response-schema.json
slug: geode-rest-server-list-response
source_filename: geode-rest-server-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-server-list-response-schema.json\",\n  \"title\": \"ServerListResponse\",\n  \"description\": \"Response containing list of Geode cache servers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"servers\": {\n      \"type\": \"array\",\n      \"description\": \"List of server addresses\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"localhost:40404\",\n        \"geode-server-02:40404\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-geode/refs/heads/main/json-schema/geode-rest-server-list-response-schema.json
tags:
- Apache
- Caching
- Data Grid
- Distributed Systems
- In-Memory
- Open Source
title: ServerListResponse
---
