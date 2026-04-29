---
description: Specifies dependency JARs, as well as JAR files that contain user-defined functions (UDF).
layout: schema
name: CustomArtifactConfiguration
properties_list:
- description: ''
  name: ArtifactType
  type: object
- description: ''
  name: S3ContentLocation
  type: object
- description: ''
  name: MavenReference
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-custom-artifact-configuration-schema.json
slug: amazon-managed-apache-flink-custom-artifact-configuration
source_filename: amazon-managed-apache-flink-custom-artifact-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-custom-artifact-configuration-schema.json\",\n  \"title\": \"CustomArtifactConfiguration\",\n  \"description\": \"Specifies dependency JARs, as well as JAR files that contain user-defined functions (UDF).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ArtifactType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactType\"\n        },\n        {\n          \"description\": \" <code>UDF</code> stands for user-defined functions. This type of artifact must be in an S3 bucket. A <code>DEPENDENCY_JAR</code> can be in either Maven or an S3 bucket.\"\n        }\n      ]\n    },\n    \"S3ContentLocation\": {\n      \"$ref\": \"#/components/schemas/S3ContentLocation\"\n    },\n    \"MavenReference\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/MavenReference\"\n        },\n        {\n          \"description\": \"The parameters required to fully specify a Maven reference.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ArtifactType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-custom-artifact-configuration-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: CustomArtifactConfiguration
---
