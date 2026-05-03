---
description: Schema representing the Retrofit type-safe HTTP client library metadata, modules, and configuration.
layout: schema
name: Retrofit Library
properties_list:
- description: The library name.
  name: name
  type: string
- description: The version of Retrofit.
  name: version
  type: string
- description: Maven Group ID.
  name: groupId
  type: string
- description: Maven Artifact ID.
  name: artifactId
  type: string
- description: Minimum required Java version.
  name: minimumJavaVersion
  type: string
- description: Minimum Android API level required.
  name: minimumAndroidApi
  type: integer
- description: Available converter modules for serialization.
  name: converters
  type: array
- description: Available call adapter modules for async frameworks.
  name: callAdapters
  type: array
- description: License identifier.
  name: license
  type: string
- description: Source code repository URL.
  name: repository
  type: string
provider_name: Retrofit
provider_slug: retrofit
schema_file: json-schema/retrofit-library-schema.json
slug: retrofit-library
source_filename: retrofit-library-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/retrofit/json-schema/retrofit-library-schema.json\",\n  \"title\": \"Retrofit Library\",\n  \"description\": \"Schema representing the Retrofit type-safe HTTP client library metadata, modules, and configuration.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"version\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The library name.\",\n      \"const\": \"retrofit\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of Retrofit.\",\n      \"examples\": [\"3.0.0\", \"2.11.0\"]\n    },\n    \"groupId\": {\n      \"type\": \"string\",\n      \"description\": \"Maven Group ID.\",\n      \"const\": \"com.squareup.retrofit2\"\n    },\n    \"artifactId\": {\n      \"type\": \"string\",\n      \"description\": \"Maven Artifact ID.\",\n      \"const\": \"retrofit\"\n \
  \   },\n    \"minimumJavaVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Minimum required Java version.\",\n      \"examples\": [\"8\", \"11\"]\n    },\n    \"minimumAndroidApi\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum Android API level required.\",\n      \"examples\": [21]\n    },\n    \"converters\": {\n      \"type\": \"array\",\n      \"description\": \"Available converter modules for serialization.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"gson\", \"moshi\", \"jackson\", \"kotlinx-serialization\", \"jaxb\", \"wire\", \"simplexml\", \"scalars\"]\n      }\n    },\n    \"callAdapters\": {\n      \"type\": \"array\",\n      \"description\": \"Available call adapter modules for async frameworks.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"rxjava\", \"rxjava2\", \"rxjava3\", \"java8\", \"guava\", \"scala\"]\n      }\n    },\n    \"license\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"License identifier.\",\n      \"const\": \"Apache-2.0\"\n    },\n    \"repository\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Source code repository URL.\",\n      \"const\": \"https://github.com/square/retrofit\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/retrofit/refs/heads/main/json-schema/retrofit-library-schema.json
tags:
- Android
- HTTP Client
- Java
- Kotlin
- Library
- Mobile
- Open Source
- SDK
- Square
title: Retrofit Library
---
