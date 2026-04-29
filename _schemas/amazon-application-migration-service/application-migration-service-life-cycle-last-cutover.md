---
description: Details about the last cutover lifecycle event
layout: schema
name: LifeCycleLastCutover
properties_list:
- description: Job ID of the last cutover
  name: jobID
  type: string
- description: Date/time the cutover was initiated
  name: initiatedDateTime
  type: string
- description: Date/time the cutover was finalized
  name: finalizedDateTime
  type: string
- description: Date/time the cutover was reverted
  name: revertedDateTime
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-life-cycle-last-cutover-schema.json
slug: application-migration-service-life-cycle-last-cutover
source_filename: application-migration-service-life-cycle-last-cutover-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-life-cycle-last-cutover-schema.json\",\n  \"title\": \"LifeCycleLastCutover\",\n  \"description\": \"Details about the last cutover lifecycle event\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobID\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID of the last cutover\"\n    },\n    \"initiatedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date/time the cutover was initiated\"\n    },\n    \"finalizedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date/time the cutover was finalized\"\n    },\n    \"revertedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date/time the cutover was reverted\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-life-cycle-last-cutover-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: LifeCycleLastCutover
---
