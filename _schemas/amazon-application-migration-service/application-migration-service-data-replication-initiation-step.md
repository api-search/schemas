---
description: A single step in the replication initiation process
layout: schema
name: DataReplicationInitiationStep
properties_list:
- description: Step name
  name: name
  type: string
- description: Step status
  name: status
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-data-replication-initiation-step-schema.json
slug: application-migration-service-data-replication-initiation-step
source_filename: application-migration-service-data-replication-initiation-step-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-data-replication-initiation-step-schema.json\",\n  \"title\": \"DataReplicationInitiationStep\",\n  \"description\": \"A single step in the replication initiation process\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Step name\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Step status\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-data-replication-initiation-step-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: DataReplicationInitiationStep
---
