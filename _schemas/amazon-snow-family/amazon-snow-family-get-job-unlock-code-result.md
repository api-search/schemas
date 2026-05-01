---
description: GetJobUnlockCodeResult schema from Amazon Snow Family API
layout: schema
name: GetJobUnlockCodeResult
properties_list:
- description: ''
  name: UnlockCode
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-get-job-unlock-code-result-schema.json
slug: amazon-snow-family-get-job-unlock-code-result
source_filename: amazon-snow-family-get-job-unlock-code-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-get-job-unlock-code-result-schema.json\",\n  \"title\": \"GetJobUnlockCodeResult\",\n  \"description\": \"GetJobUnlockCodeResult schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UnlockCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>UnlockCode</code> value for the specified job. The <code>UnlockCode</code> value can be accessed for up to 360 days after the job has been created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-get-job-unlock-code-result-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: GetJobUnlockCodeResult
---
