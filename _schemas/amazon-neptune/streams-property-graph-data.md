---
description: The serialized property graph change data. The type field indicates the element kind.
layout: schema
name: PropertyGraphData
properties_list:
- description: The unique identifier of the element.
  name: id
  type: string
- description: 'The element type: v (vertex), vl (vertex label), vp (vertex property), e (edge), ep (edge property).'
  name: type
  type: string
- description: The property key name.
  name: key
  type: string
- description: The property value with its data type.
  name: value
  type: object
- description: Source vertex ID (for edges only).
  name: from
  type: string
- description: Target vertex ID (for edges only).
  name: to
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/streams-property-graph-data-schema.json
slug: streams-property-graph-data
source_filename: streams-property-graph-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/streams-property-graph-data-schema.json\",\n  \"title\": \"PropertyGraphData\",\n  \"description\": \"The serialized property graph change data. The type field indicates the element kind.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the element.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The element type: v (vertex), vl (vertex label), vp (vertex property), e (edge), ep (edge property).\",\n      \"enum\": [\n        \"v\",\n        \"vl\",\n        \"vp\",\n        \"e\",\n        \"ep\"\n      ]\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The property key name.\"\n    },\n    \"value\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"The property value with its data type.\",\n      \"properties\": {\n        \"value\": {\n          \"description\": \"The actual property value.\"\n        },\n        \"dataType\": {\n          \"type\": \"string\",\n          \"description\": \"The data type (String, Integer, Double, etc.).\"\n        }\n      }\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"Source vertex ID (for edges only).\"\n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"description\": \"Target vertex ID (for edges only).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/streams-property-graph-data-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: PropertyGraphData
---
