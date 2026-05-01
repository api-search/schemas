---
description: GetJobManifestResult schema from Amazon Snow Family API
layout: schema
name: GetJobManifestResult
properties_list:
- description: ''
  name: ManifestURI
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-get-job-manifest-result-schema.json
slug: amazon-snow-family-get-job-manifest-result
source_filename: amazon-snow-family-get-job-manifest-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-get-job-manifest-result-schema.json\",\n  \"title\": \"GetJobManifestResult\",\n  \"description\": \"GetJobManifestResult schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ManifestURI\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon S3 presigned URL for the manifest file associated with the specified <code>JobId</code> value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-get-job-manifest-result-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: GetJobManifestResult
---
