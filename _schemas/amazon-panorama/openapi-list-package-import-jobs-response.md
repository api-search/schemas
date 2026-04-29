---
description: ListPackageImportJobsResponse schema from Amazon Panorama
layout: schema
name: ListPackageImportJobsResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: PackageImportJobs
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-list-package-import-jobs-response-schema.json
slug: openapi-list-package-import-jobs-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-list-package-import-jobs-response-schema.json\",\n  \"title\": \"ListPackageImportJobsResponse\",\n  \"description\": \"ListPackageImportJobsResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A pagination token that's included if more results are available.\"\n        }\n      ]\n    },\n    \"PackageImportJobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageImportJobList\"\n        },\n        {\n          \"description\": \"A list of package import jobs.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PackageImportJobs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-list-package-import-jobs-response-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: ListPackageImportJobsResponse
---
