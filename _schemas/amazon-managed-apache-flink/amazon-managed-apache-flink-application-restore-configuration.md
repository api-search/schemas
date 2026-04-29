---
description: Specifies the method and snapshot to use when restarting an application using previously saved application state.
layout: schema
name: ApplicationRestoreConfiguration
properties_list:
- description: ''
  name: ApplicationRestoreType
  type: object
- description: ''
  name: SnapshotName
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-application-restore-configuration-schema.json
slug: amazon-managed-apache-flink-application-restore-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-restore-configuration-schema.json\",\n  \"title\": \"ApplicationRestoreConfiguration\",\n  \"description\": \"Specifies the method and snapshot to use when restarting an application using previously saved application state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationRestoreType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationRestoreType\"\n        },\n        {\n          \"description\": \"Specifies how the application should be restored.\"\n        }\n      ]\n    },\n    \"SnapshotName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotName\"\n        },\n        {\n          \"description\": \"The identifier of an existing snapshot of application\
  \ state to use to restart an application. The application uses this value if <code>RESTORE_FROM_CUSTOM_SNAPSHOT</code> is specified for the <code>ApplicationRestoreType</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationRestoreType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-restore-configuration-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ApplicationRestoreConfiguration
---
