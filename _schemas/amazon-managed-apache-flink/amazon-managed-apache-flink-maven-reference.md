---
description: The information required to specify a Maven reference. You can use Maven references to specify dependency JAR files.
layout: schema
name: MavenReference
properties_list:
- description: ''
  name: GroupId
  type: object
- description: ''
  name: ArtifactId
  type: object
- description: ''
  name: Version
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-maven-reference-schema.json
slug: amazon-managed-apache-flink-maven-reference
source_filename: amazon-managed-apache-flink-maven-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-maven-reference-schema.json\",\n  \"title\": \"MavenReference\",\n  \"description\": \"The information required to specify a Maven reference. You can use Maven references to specify dependency JAR files.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MavenGroupId\"\n        },\n        {\n          \"description\": \"The group ID of the Maven reference.\"\n        }\n      ]\n    },\n    \"ArtifactId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MavenArtifactId\"\n        },\n        {\n          \"description\": \"The artifact ID of the Maven reference.\"\n        }\n      ]\n    },\n    \"Version\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/MavenVersion\"\n        },\n        {\n          \"description\": \"The version of the Maven reference.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GroupId\",\n    \"ArtifactId\",\n    \"Version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-maven-reference-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: MavenReference
---
