---
description: Schema describing JSON Patch (RFC 6902) operations for modifying JSON documents, and JSON Merge Patch (RFC 7396) for merging partial updates into JSON documents.
layout: schema
name: JSON Patch and JSON Merge Patch
properties_list: []
provider_name: JSON
provider_slug: json
schema_file: json-schema/json-patch.json
slug: json-patch
source_filename: json-patch.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"json-patch.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JSON Patch and JSON Merge Patch\",\n  \"description\": \"Schema describing JSON Patch (RFC 6902) operations for modifying JSON documents, and JSON Merge Patch (RFC 7396) for merging partial updates into JSON documents.\",\n  \"oneOf\": [\n    {\n      \"$ref\": \"#/$defs/jsonPatch\"\n    },\n    {\n      \"$ref\": \"#/$defs/jsonMergePatch\"\n    }\n  ],\n  \"$defs\": {\n    \"jsonPatch\": {\n      \"title\": \"JSON Patch (RFC 6902)\",\n      \"description\": \"A JSON Patch document is a JSON document that represents an array of operations to apply to a target JSON document.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/operation\"\n      },\n      \"minItems\": 1\n    },\n    \"operation\": {\n      \"type\": \"object\",\n      \"description\": \"A single JSON Patch operation.\",\n      \"required\": [\n        \"op\",\n    \
  \    \"path\"\n      ],\n      \"properties\": {\n        \"op\": {\n          \"type\": \"string\",\n          \"description\": \"The operation to perform.\",\n          \"enum\": [\n            \"add\",\n            \"remove\",\n            \"replace\",\n            \"move\",\n            \"copy\",\n            \"test\"\n          ]\n        },\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"A JSON Pointer (RFC 6901) string identifying the target location within the document.\",\n          \"examples\": [\n            \"/foo/bar\",\n            \"/items/0\",\n            \"/~0escaped~1path\"\n          ]\n        },\n        \"value\": {\n          \"description\": \"The value to use for add, replace, or test operations.\"\n        },\n        \"from\": {\n          \"type\": \"string\",\n          \"description\": \"A JSON Pointer string identifying the source location for move or copy operations.\",\n          \"examples\": [\n            \"/foo/bar\"\
  \n          ]\n        }\n      },\n      \"allOf\": [\n        {\n          \"if\": {\n            \"properties\": {\n              \"op\": {\n                \"enum\": [\"add\", \"replace\", \"test\"]\n              }\n            }\n          },\n          \"then\": {\n            \"required\": [\"value\"]\n          }\n        },\n        {\n          \"if\": {\n            \"properties\": {\n              \"op\": {\n                \"enum\": [\"move\", \"copy\"]\n              }\n            }\n          },\n          \"then\": {\n            \"required\": [\"from\"]\n          }\n        }\n      ],\n      \"additionalProperties\": false\n    },\n    \"jsonMergePatch\": {\n      \"title\": \"JSON Merge Patch (RFC 7396)\",\n      \"description\": \"A JSON Merge Patch document describes changes to a target JSON document using a syntax that closely mirrors the document being modified. Recipients process merge patches by comparing the content with the current target document: members\
  \ present in the patch replace the corresponding target values, null values remove the corresponding target members, and members not present in the patch remain unchanged.\",\n      \"oneOf\": [\n        {\n          \"type\": \"object\",\n          \"description\": \"An object whose members represent changes to apply. A null value removes the member; an object value is applied recursively; any other value replaces the target member.\",\n          \"additionalProperties\": true\n        },\n        {\n          \"type\": \"array\",\n          \"description\": \"When the merge patch is not an object, the entire target is replaced.\"\n        },\n        {\n          \"type\": \"string\",\n          \"description\": \"When the merge patch is not an object, the entire target is replaced.\"\n        },\n        {\n          \"type\": \"number\",\n          \"description\": \"When the merge patch is not an object, the entire target is replaced.\"\n        },\n        {\n          \"type\":\
  \ \"boolean\",\n          \"description\": \"When the merge patch is not an object, the entire target is replaced.\"\n        },\n        {\n          \"type\": \"null\",\n          \"description\": \"A null merge patch replaces the entire target with null.\"\n        }\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/json/refs/heads/main/json-schema/json-patch.json
tags:
- Data Format
- Serialization
- Web Development
- JSON
- RFC 8259
title: JSON Patch and JSON Merge Patch
---
