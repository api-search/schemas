---
description: Specifies a dependency JAR or a JAR of user-defined functions.
layout: schema
name: CustomArtifactConfigurationDescription
properties_list:
- description: ''
  name: ArtifactType
  type: object
- description: ''
  name: S3ContentLocationDescription
  type: object
- description: ''
  name: MavenReferenceDescription
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-custom-artifact-configuration-description-schema.json
slug: amazon-managed-apache-flink-custom-artifact-configuration-description
source_filename: amazon-managed-apache-flink-custom-artifact-configuration-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-custom-artifact-configuration-description-schema.json\",\n  \"title\": \"CustomArtifactConfigurationDescription\",\n  \"description\": \"Specifies a dependency JAR or a JAR of user-defined functions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ArtifactType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactType\"\n        },\n        {\n          \"description\": \" <code>UDF</code> stands for user-defined functions. This type of artifact must be in an S3 bucket. A <code>DEPENDENCY_JAR</code> can be in either Maven or an S3 bucket.\"\n        }\n      ]\n    },\n    \"S3ContentLocationDescription\": {\n      \"$ref\": \"#/components/schemas/S3ContentLocation\"\n    },\n    \"MavenReferenceDescription\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MavenReference\"\n        },\n        {\n          \"description\": \"The parameters that are required to specify a Maven dependency.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-custom-artifact-configuration-description-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: CustomArtifactConfigurationDescription
---
