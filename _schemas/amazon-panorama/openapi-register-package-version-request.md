---
description: RegisterPackageVersionRequest schema from Amazon Panorama
layout: schema
name: RegisterPackageVersionRequest
properties_list:
- description: ''
  name: MarkLatest
  type: object
- description: ''
  name: OwnerAccount
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-register-package-version-request-schema.json
slug: openapi-register-package-version-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-register-package-version-request-schema.json\",\n  \"title\": \"RegisterPackageVersionRequest\",\n  \"description\": \"RegisterPackageVersionRequest schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MarkLatest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MarkLatestPatch\"\n        },\n        {\n          \"description\": \"Whether to mark the new version as the latest version.\"\n        }\n      ]\n    },\n    \"OwnerAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageOwnerAccount\"\n        },\n        {\n          \"description\": \"An owner account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-register-package-version-request-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: RegisterPackageVersionRequest
---
