---
description: Schema describing the proto3 JSON encoding rules for Protocol Buffers messages. Proto3 JSON mapping defines how protobuf scalar types, well-known types, and composite types are represented in JSON format as specified by the Protocol Buffers Language Guide.
layout: schema
name: Protocol Buffers JSON Mapping
properties_list:
- description: A protobuf message serialized to JSON. Each field uses its proto field name in lowerCamelCase as the JSON key. Fields with default values are omitted by default.
  name: message
  type: object
- description: The type URL for google.protobuf.Any messages, identifying the packed message type (e.g., type.googleapis.com/package.MessageName).
  name: '@type'
  type: string
- description: The value field used by wrapper types (e.g., google.protobuf.StringValue, google.protobuf.Int32Value) and google.protobuf.Value.
  name: value
  type: object
provider_name: Protocol Buffers
provider_slug: protocol-buffers
schema_file: json-schema/protocol-buffers-json-mapping.json
slug: protocol-buffers-json-mapping
source_filename: protocol-buffers-json-mapping.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"protobuf-json-mapping.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Protocol Buffers JSON Mapping\",\n  \"description\": \"Schema describing the proto3 JSON encoding rules for Protocol Buffers messages. Proto3 JSON mapping defines how protobuf scalar types, well-known types, and composite types are represented in JSON format as specified by the Protocol Buffers Language Guide.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"object\",\n      \"description\": \"A protobuf message serialized to JSON. Each field uses its proto field name in lowerCamelCase as the JSON key. Fields with default values are omitted by default.\",\n      \"additionalProperties\": true\n    },\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The type URL for google.protobuf.Any messages, identifying the packed message type (e.g., type.googleapis.com/package.MessageName).\",\n   \
  \   \"format\": \"uri\",\n      \"examples\": [\n        \"type.googleapis.com/google.protobuf.Duration\",\n        \"type.googleapis.com/google.protobuf.Struct\"\n      ]\n    },\n    \"value\": {\n      \"description\": \"The value field used by wrapper types (e.g., google.protobuf.StringValue, google.protobuf.Int32Value) and google.protobuf.Value.\"\n    }\n  },\n  \"definitions\": {\n    \"Duration\": {\n      \"type\": \"string\",\n      \"description\": \"google.protobuf.Duration encoded as a string with suffix 's' for seconds (e.g., '3.5s'). Nanosecond precision is supported.\",\n      \"pattern\": \"^-?[0-9]+(\\\\.[0-9]+)?s$\",\n      \"examples\": [\"1.5s\", \"0.001s\", \"-42s\"]\n    },\n    \"Timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"google.protobuf.Timestamp encoded as an RFC 3339 date-time string in UTC with suffix 'Z'.\",\n      \"format\": \"date-time\",\n      \"examples\": [\"2025-01-15T12:00:00Z\", \"2025-06-01T00:00:00.000Z\"]\n    },\n  \
  \  \"FieldMask\": {\n      \"type\": \"string\",\n      \"description\": \"google.protobuf.FieldMask encoded as a single comma-delimited string of field paths in lowerCamelCase.\",\n      \"examples\": [\"fieldOne,fieldTwo.subField\", \"name,displayName\"]\n    },\n    \"Struct\": {\n      \"type\": \"object\",\n      \"description\": \"google.protobuf.Struct encoded as a regular JSON object with string keys and google.protobuf.Value values.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/definitions/Value\"\n      }\n    },\n    \"Value\": {\n      \"description\": \"google.protobuf.Value can represent any JSON value: null, number, string, boolean, struct, or list.\",\n      \"oneOf\": [\n        { \"type\": \"null\" },\n        { \"type\": \"number\" },\n        { \"type\": \"string\" },\n        { \"type\": \"boolean\" },\n        { \"type\": \"object\", \"additionalProperties\": true },\n        { \"type\": \"array\" }\n      ]\n    },\n    \"ListValue\": {\n      \"type\"\
  : \"array\",\n      \"description\": \"google.protobuf.ListValue encoded as a JSON array of google.protobuf.Value elements.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Value\"\n      }\n    },\n    \"NullValue\": {\n      \"type\": \"null\",\n      \"description\": \"google.protobuf.NullValue is always encoded as JSON null.\"\n    },\n    \"Empty\": {\n      \"type\": \"object\",\n      \"description\": \"google.protobuf.Empty encoded as an empty JSON object.\",\n      \"additionalProperties\": false\n    },\n    \"Int64Value\": {\n      \"type\": \"string\",\n      \"description\": \"64-bit integer types (int64, uint64, sint64, fixed64, sfixed64) are encoded as decimal strings in JSON to preserve precision.\",\n      \"pattern\": \"^-?[0-9]+$\"\n    },\n    \"BytesValue\": {\n      \"type\": \"string\",\n      \"description\": \"The bytes scalar type is encoded as a base64-encoded string using standard base64 encoding with padding.\",\n      \"contentEncoding\": \"base64\"\
  \n    },\n    \"EnumValue\": {\n      \"description\": \"Enum values are encoded as the string name of the enum value. If unrecognized, the integer value is used instead.\",\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"integer\" }\n      ]\n    },\n    \"RepeatedField\": {\n      \"type\": \"array\",\n      \"description\": \"Repeated fields are encoded as JSON arrays. An empty repeated field may be omitted or represented as an empty array.\"\n    },\n    \"MapField\": {\n      \"type\": \"object\",\n      \"description\": \"Map fields are encoded as JSON objects. Map keys are always converted to strings. Sort order is not guaranteed.\",\n      \"additionalProperties\": true\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/protocol-buffers/refs/heads/main/json-schema/protocol-buffers-json-mapping.json
tags:
- Data Format
- gRPC
- Protobuf
- Protocol Buffers
- Serialization
title: Protocol Buffers JSON Mapping
---
