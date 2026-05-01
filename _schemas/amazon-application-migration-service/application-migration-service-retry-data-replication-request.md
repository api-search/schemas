---
description: Request to retry data replication
layout: schema
name: RetryDataReplicationRequest
properties_list:
- description: Source server ID to retry replication for
  name: sourceServerID
  type: string
- description: Account ID for cross-account access
  name: accountID
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-retry-data-replication-request-schema.json
slug: application-migration-service-retry-data-replication-request
source_filename: application-migration-service-retry-data-replication-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-retry-data-replication-request-schema.json\",\n  \"title\": \"RetryDataReplicationRequest\",\n  \"description\": \"Request to retry data replication\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceServerID\": {\n      \"type\": \"string\",\n      \"description\": \"Source server ID to retry replication for\"\n    },\n    \"accountID\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID for cross-account access\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-retry-data-replication-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: RetryDataReplicationRequest
---
