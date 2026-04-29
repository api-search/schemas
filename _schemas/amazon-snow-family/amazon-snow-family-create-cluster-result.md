---
description: CreateClusterResult schema from Amazon Snow Family API
layout: schema
name: CreateClusterResult
properties_list:
- description: ''
  name: ClusterId
  type: object
- description: ''
  name: JobListEntries
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-create-cluster-result-schema.json
slug: amazon-snow-family-create-cluster-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-cluster-result-schema.json\",\n  \"title\": \"CreateClusterResult\",\n  \"description\": \"CreateClusterResult schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClusterId\"\n        },\n        {\n          \"description\": \"The automatically generated ID for a cluster.\"\n        }\n      ]\n    },\n    \"JobListEntries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobListEntryList\"\n        },\n        {\n          \"description\": \"List of jobs created for this cluster. For syntax, see <a href=\\\"http://amazonaws.com/snowball/latest/api-reference/API_ListJobs.html#API_ListJobs_ResponseSyntax\\\">ListJobsResult$JobListEntries</a>\
  \ in this guide.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-cluster-result-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: CreateClusterResult
---
