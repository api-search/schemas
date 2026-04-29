---
description: ListHarvestJobsResponse schema from Amazon MediaPackage API
layout: schema
name: ListHarvestJobsResponse
properties_list:
- description: ''
  name: HarvestJobs
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-list-harvest-jobs-response-schema.json
slug: mediapackage-api-list-harvest-jobs-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-list-harvest-jobs-response-schema.json\",\n  \"title\": \"ListHarvestJobsResponse\",\n  \"description\": \"ListHarvestJobsResponse schema from Amazon MediaPackage API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HarvestJobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfHarvestJob\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"harvestJobs\"\n          },\n          \"description\": \"A list of HarvestJob records.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"A token that can be used to resume\
  \ pagination from the end of the collection.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-list-harvest-jobs-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListHarvestJobsResponse
---
