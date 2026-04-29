---
description: Replication error details
layout: schema
name: DataReplicationError
properties_list:
- description: Error type
  name: error
  type: string
- description: Raw error message
  name: rawError
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-data-replication-error-schema.json
slug: application-migration-service-data-replication-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-data-replication-error-schema.json\",\n  \"title\": \"DataReplicationError\",\n  \"description\": \"Replication error details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error type\"\n    },\n    \"rawError\": {\n      \"type\": \"string\",\n      \"description\": \"Raw error message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-data-replication-error-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: DataReplicationError
---
