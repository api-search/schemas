---
description: Response containing the total count of packages and an array of package detail objects for the specified application.
layout: schema
name: PackageListResponse
properties_list:
- description: The total number of in-flight packages for the application. Maximum of 100.
  name: totalPackageCount
  type: integer
- description: Array of package objects ordered by last modified timestamp, newest first.
  name: packages
  type: array
provider_name: Appian
provider_slug: appian
schema_file: json-schema/application-package-details-package-list-response-schema.json
slug: application-package-details-package-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/application-package-details-package-list-response-schema.json\",\n  \"title\": \"PackageListResponse\",\n  \"description\": \"Response containing the total count of packages and an array of package detail objects for the specified application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalPackageCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of in-flight packages for the application. Maximum of 100.\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"example\": 3\n    },\n    \"packages\": {\n      \"type\": \"array\",\n      \"description\": \"Array of package objects ordered by last modified timestamp, newest first.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Package\"\n      }\n    }\n  },\n  \"required\": [\n    \"totalPackageCount\"\
  ,\n    \"packages\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/application-package-details-package-list-response-schema.json
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: PackageListResponse
---
