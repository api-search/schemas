---
description: A sequence identifier for a stream event.
layout: schema
name: StreamEventId
properties_list:
- description: The commit (transaction) number.
  name: commitNum
  type: integer
- description: The operation number within the commit.
  name: opNum
  type: integer
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/streams-stream-event-id-schema.json
slug: streams-stream-event-id
source_filename: streams-stream-event-id-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/streams-stream-event-id-schema.json\",\n  \"title\": \"StreamEventId\",\n  \"description\": \"A sequence identifier for a stream event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"commitNum\": {\n      \"type\": \"integer\",\n      \"description\": \"The commit (transaction) number.\"\n    },\n    \"opNum\": {\n      \"type\": \"integer\",\n      \"description\": \"The operation number within the commit.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/streams-stream-event-id-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: StreamEventId
---
