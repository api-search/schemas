---
description: Describes an update to the code of an application. Not supported for Apache Zeppelin.
layout: schema
name: CodeContentUpdate
properties_list:
- description: ''
  name: TextContentUpdate
  type: object
- description: ''
  name: ZipFileContentUpdate
  type: object
- description: ''
  name: S3ContentLocationUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-code-content-update-schema.json
slug: amazon-managed-apache-flink-code-content-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-code-content-update-schema.json\",\n  \"title\": \"CodeContentUpdate\",\n  \"description\": \"Describes an update to the code of an application. Not supported for Apache Zeppelin.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TextContentUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TextContent\"\n        },\n        {\n          \"description\": \"Describes an update to the text code for an application.\"\n        }\n      ]\n    },\n    \"ZipFileContentUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ZipFileContent\"\n        },\n        {\n          \"description\": \"Describes an update to the zipped code for an application.\"\n        }\n      ]\n    },\n    \"S3ContentLocationUpdate\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ContentLocationUpdate\"\n        },\n        {\n          \"description\": \"Describes an update to the location of code for an application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-code-content-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: CodeContentUpdate
---
