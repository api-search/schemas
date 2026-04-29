---
description: Filters for describing jobs
layout: schema
name: DescribeJobsRequestFilters
properties_list:
- description: Filter by job IDs
  name: jobIDs
  type: array
- description: Filter by start date
  name: fromDate
  type: string
- description: Filter by end date
  name: toDate
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-describe-jobs-request-filters-schema.json
slug: application-migration-service-describe-jobs-request-filters
source_filename: application-migration-service-describe-jobs-request-filters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-describe-jobs-request-filters-schema.json\",\n  \"title\": \"DescribeJobsRequestFilters\",\n  \"description\": \"Filters for describing jobs\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobIDs\": {\n      \"type\": \"array\",\n      \"description\": \"Filter by job IDs\"\n    },\n    \"fromDate\": {\n      \"type\": \"string\",\n      \"description\": \"Filter by start date\"\n    },\n    \"toDate\": {\n      \"type\": \"string\",\n      \"description\": \"Filter by end date\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-describe-jobs-request-filters-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: DescribeJobsRequestFilters
---
