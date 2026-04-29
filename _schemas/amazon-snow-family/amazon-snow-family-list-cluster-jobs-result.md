---
description: ListClusterJobsResult schema from Amazon Snow Family API
layout: schema
name: ListClusterJobsResult
properties_list:
- description: ''
  name: JobListEntries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-list-cluster-jobs-result-schema.json
slug: amazon-snow-family-list-cluster-jobs-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-cluster-jobs-result-schema.json\",\n  \"title\": \"ListClusterJobsResult\",\n  \"description\": \"ListClusterJobsResult schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobListEntries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobListEntryList\"\n        },\n        {\n          \"description\": \"Each <code>JobListEntry</code> object contains a job's state, a job's ID, and a value that indicates whether the job is a job part, in the case of export jobs. \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"HTTP requests are stateless. If you use the automatically\
  \ generated <code>NextToken</code> value in your next <code>ListClusterJobsResult</code> call, your list of returned jobs will start from this point in the array.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-cluster-jobs-result-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: ListClusterJobsResult
---
