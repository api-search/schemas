---
description: Filters for describing source servers
layout: schema
name: DescribeSourceServersRequestFilters
properties_list:
- description: Filter by source server IDs
  name: sourceServerIDs
  type: array
- description: Filter by archived status
  name: isArchived
  type: boolean
- description: Filter by replication type
  name: replicationTypes
  type: array
- description: Filter by lifecycle states
  name: lifeCycleStates
  type: array
- description: Filter by application IDs
  name: applicationIDs
  type: array
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-describe-source-servers-request-filters-schema.json
slug: application-migration-service-describe-source-servers-request-filters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-describe-source-servers-request-filters-schema.json\",\n  \"title\": \"DescribeSourceServersRequestFilters\",\n  \"description\": \"Filters for describing source servers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceServerIDs\": {\n      \"type\": \"array\",\n      \"description\": \"Filter by source server IDs\"\n    },\n    \"isArchived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Filter by archived status\"\n    },\n    \"replicationTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Filter by replication type\"\n    },\n    \"lifeCycleStates\": {\n      \"type\": \"array\",\n      \"description\": \"Filter by lifecycle states\"\n    },\n    \"applicationIDs\": {\n      \"type\": \"array\",\n      \"description\": \"Filter by application\
  \ IDs\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-describe-source-servers-request-filters-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: DescribeSourceServersRequestFilters
---
