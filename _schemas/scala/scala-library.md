---
description: Schema representing a Scala library or framework, including its build tool coordinates, compatibility, and classification.
layout: schema
name: Scala Library
properties_list:
- description: Human-readable library name.
  name: name
  type: string
- description: Brief description of the library's purpose.
  name: description
  type: string
- description: Maven/sbt group identifier.
  name: groupId
  type: string
- description: Maven/sbt artifact identifier (without Scala version suffix).
  name: artifactId
  type: string
- description: Latest stable release version.
  name: currentVersion
  type: string
- description: Supported Scala versions.
  name: scalaVersions
  type: array
- description: Supported Scala runtimes.
  name: runtimes
  type: array
- description: Primary category of the library.
  name: category
  type: string
- description: Open source license identifier.
  name: license
  type: string
- description: GitHub repository URL.
  name: githubUrl
  type: string
- description: Official documentation URL.
  name: documentationUrl
  type: string
- description: sbt library dependency declaration.
  name: sbtDependency
  type: string
- description: Key transitive dependencies.
  name: dependencies
  type: array
- description: Effect system this library integrates with (if any).
  name: effectSystem
  type: string
- description: Classification tags.
  name: tags
  type: array
provider_name: Scala
provider_slug: scala
schema_file: json-schema/scala-library-schema.json
slug: scala-library
source_filename: scala-library-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.com/schemas/scala/library\",\n  \"title\": \"Scala Library\",\n  \"description\": \"Schema representing a Scala library or framework, including its build tool coordinates, compatibility, and classification.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"groupId\", \"artifactId\", \"currentVersion\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable library name.\",\n      \"example\": \"Cats\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Brief description of the library's purpose.\"\n    },\n    \"groupId\": {\n      \"type\": \"string\",\n      \"description\": \"Maven/sbt group identifier.\",\n      \"example\": \"org.typelevel\"\n    },\n    \"artifactId\": {\n      \"type\": \"string\",\n      \"description\": \"Maven/sbt artifact identifier (without Scala version\
  \ suffix).\",\n      \"example\": \"cats-core\"\n    },\n    \"currentVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Latest stable release version.\",\n      \"example\": \"2.12.0\"\n    },\n    \"scalaVersions\": {\n      \"type\": \"array\",\n      \"description\": \"Supported Scala versions.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"2.12\", \"2.13\", \"3\"]\n      },\n      \"example\": [\"2.13\", \"3\"]\n    },\n    \"runtimes\": {\n      \"type\": \"array\",\n      \"description\": \"Supported Scala runtimes.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"jvm\", \"js\", \"native\"]\n      },\n      \"example\": [\"jvm\", \"js\", \"native\"]\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"functional-programming\",\n        \"effect-system\",\n        \"http\",\n        \"database\",\n        \"json\",\n        \"streaming\",\n        \"testing\",\n        \"build-tool\"\
  ,\n        \"actor-model\",\n        \"big-data\",\n        \"logging\",\n        \"serialization\",\n        \"configuration\",\n        \"other\"\n      ],\n      \"description\": \"Primary category of the library.\"\n    },\n    \"license\": {\n      \"type\": \"string\",\n      \"description\": \"Open source license identifier.\",\n      \"example\": \"Apache-2.0\"\n    },\n    \"githubUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"GitHub repository URL.\"\n    },\n    \"documentationUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Official documentation URL.\"\n    },\n    \"sbtDependency\": {\n      \"type\": \"string\",\n      \"description\": \"sbt library dependency declaration.\",\n      \"example\": \"\\\"org.typelevel\\\" %% \\\"cats-core\\\" % \\\"2.12.0\\\"\"\n    },\n    \"dependencies\": {\n      \"type\": \"array\",\n      \"description\": \"Key transitive dependencies.\",\n      \"\
  items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"effectSystem\": {\n      \"type\": \"string\",\n      \"enum\": [\"cats-effect\", \"zio\", \"monix\", \"futures\", \"none\"],\n      \"description\": \"Effect system this library integrates with (if any).\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Classification tags.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scala/refs/heads/main/json-schema/scala-library-schema.json
tags:
- Big Data
- Distributed Systems
- Functional Programming
- JVM
- Programming Language
- Scala
- Scala 3
- Type Safety
title: Scala Library
---
