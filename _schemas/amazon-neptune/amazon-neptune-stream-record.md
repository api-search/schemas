---
description: Represents a change-log stream record from Neptune Streams. Each record captures a single mutation (ADD or REMOVE) made to graph data. Supports both property graph (PG_JSON format) and RDF (NQUADS format) records.
layout: schema
name: Amazon Neptune Stream Record
properties_list:
- description: The sequence identifier of the last change in the response.
  name: lastEventId
  type: object
- description: Unix epoch timestamp in milliseconds of the last transaction commit.
  name: lastTrxTimestamp
  type: integer
- description: The serialization format of the stream records.
  name: format
  type: string
- description: The array of change-log stream records.
  name: records
  type: array
- description: The total number of records in the response.
  name: totalRecords
  type: integer
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/amazon-neptune-stream-record-schema.json
slug: amazon-neptune-stream-record
source_filename: amazon-neptune-stream-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/amazon-neptune/json-schema/amazon-neptune-stream-record-schema.json\",\n  \"title\": \"Amazon Neptune Stream Record\",\n  \"description\": \"Represents a change-log stream record from Neptune Streams. Each record captures a single mutation (ADD or REMOVE) made to graph data. Supports both property graph (PG_JSON format) and RDF (NQUADS format) records.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"lastEventId\",\n    \"lastTrxTimestamp\",\n    \"format\",\n    \"records\",\n    \"totalRecords\"\n  ],\n  \"properties\": {\n    \"lastEventId\": {\n      \"$ref\": \"#/$defs/EventId\",\n      \"description\": \"The sequence identifier of the last change in the response.\"\n    },\n    \"lastTrxTimestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix epoch timestamp in milliseconds of the last transaction commit.\"\n    },\n    \"format\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The serialization format of the stream records.\",\n      \"enum\": [\n        \"PG_JSON\",\n        \"NQUADS\"\n      ]\n    },\n    \"records\": {\n      \"type\": \"array\",\n      \"description\": \"The array of change-log stream records.\",\n      \"items\": {\n        \"oneOf\": [\n          { \"$ref\": \"#/$defs/PropertyGraphRecord\" },\n          { \"$ref\": \"#/$defs/SparqlRecord\" }\n        ]\n      }\n    },\n    \"totalRecords\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of records in the response.\"\n    }\n  },\n  \"$defs\": {\n    \"EventId\": {\n      \"type\": \"object\",\n      \"title\": \"Stream Event ID\",\n      \"description\": \"A unique sequence identifier for a stream event, composed of the commit number and operation number.\",\n      \"required\": [\n        \"commitNum\",\n        \"opNum\"\n      ],\n      \"properties\": {\n        \"commitNum\": {\n          \"type\"\
  : \"integer\",\n          \"description\": \"The commit (transaction) number.\"\n        },\n        \"opNum\": {\n          \"type\": \"integer\",\n          \"description\": \"The operation number within the commit.\"\n        }\n      }\n    },\n    \"PropertyGraphRecord\": {\n      \"type\": \"object\",\n      \"title\": \"Property Graph Stream Record\",\n      \"description\": \"A change record for property graph (Gremlin/openCypher) data in PG_JSON format.\",\n      \"required\": [\n        \"commitTimestamp\",\n        \"eventId\",\n        \"data\",\n        \"op\"\n      ],\n      \"properties\": {\n        \"commitTimestamp\": {\n          \"type\": \"integer\",\n          \"description\": \"Unix epoch timestamp in milliseconds of the transaction commit.\"\n        },\n        \"eventId\": {\n          \"$ref\": \"#/$defs/EventId\"\n        },\n        \"data\": {\n          \"$ref\": \"#/$defs/PropertyGraphData\"\n        },\n        \"op\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The operation type.\",\n          \"enum\": [\n            \"ADD\",\n            \"REMOVE\"\n          ]\n        },\n        \"isLastOp\": {\n          \"type\": \"boolean\",\n          \"description\": \"True only if this is the last operation in the transaction.\"\n        }\n      }\n    },\n    \"PropertyGraphData\": {\n      \"type\": \"object\",\n      \"title\": \"Property Graph Data\",\n      \"description\": \"The property graph change data within a stream record.\",\n      \"required\": [\n        \"id\",\n        \"type\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the graph element.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of graph element: v (vertex), vl (vertex label), vp (vertex property), e (edge), ep (edge property).\",\n          \"enum\": [\n            \"v\",\n           \
  \ \"vl\",\n            \"vp\",\n            \"e\",\n            \"ep\"\n          ]\n        },\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The property key name (for property changes).\"\n        },\n        \"value\": {\n          \"type\": \"object\",\n          \"description\": \"The typed property value.\",\n          \"properties\": {\n            \"value\": {\n              \"description\": \"The actual value.\"\n            },\n            \"dataType\": {\n              \"type\": \"string\",\n              \"description\": \"The Neptune data type.\",\n              \"enum\": [\n                \"String\",\n                \"Integer\",\n                \"Long\",\n                \"Double\",\n                \"Float\",\n                \"Boolean\",\n                \"Date\",\n                \"DateTime\"\n              ]\n            }\n          }\n        },\n        \"from\": {\n          \"type\": \"string\",\n          \"description\":\
  \ \"The source vertex ID (for edge records only).\"\n        },\n        \"to\": {\n          \"type\": \"string\",\n          \"description\": \"The target vertex ID (for edge records only).\"\n        }\n      }\n    },\n    \"SparqlRecord\": {\n      \"type\": \"object\",\n      \"title\": \"SPARQL Stream Record\",\n      \"description\": \"A change record for RDF (SPARQL) data in NQUADS format.\",\n      \"required\": [\n        \"commitTimestamp\",\n        \"eventId\",\n        \"data\",\n        \"op\"\n      ],\n      \"properties\": {\n        \"commitTimestamp\": {\n          \"type\": \"integer\",\n          \"description\": \"Unix epoch timestamp in milliseconds of the transaction commit.\"\n        },\n        \"eventId\": {\n          \"$ref\": \"#/$defs/EventId\"\n        },\n        \"data\": {\n          \"type\": \"object\",\n          \"required\": [\n            \"stmt\"\n          ],\n          \"properties\": {\n            \"stmt\": {\n              \"type\": \"\
  string\",\n              \"description\": \"The N-Quads statement representing the RDF triple or quad change.\"\n            }\n          }\n        },\n        \"op\": {\n          \"type\": \"string\",\n          \"description\": \"The operation type.\",\n          \"enum\": [\n            \"ADD\",\n            \"REMOVE\"\n          ]\n        },\n        \"isLastOp\": {\n          \"type\": \"boolean\",\n          \"description\": \"True only if this is the last operation in the transaction.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/amazon-neptune-stream-record-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: Amazon Neptune Stream Record
---
