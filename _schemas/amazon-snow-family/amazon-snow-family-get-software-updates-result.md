---
description: GetSoftwareUpdatesResult schema from Amazon Snow Family API
layout: schema
name: GetSoftwareUpdatesResult
properties_list:
- description: ''
  name: UpdatesURI
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-get-software-updates-result-schema.json
slug: amazon-snow-family-get-software-updates-result
source_filename: amazon-snow-family-get-software-updates-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-get-software-updates-result-schema.json\",\n  \"title\": \"GetSoftwareUpdatesResult\",\n  \"description\": \"GetSoftwareUpdatesResult schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UpdatesURI\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon S3 presigned URL for the update file associated with the specified <code>JobId</code> value. The software update will be available for 2 days after this request is made. To access an update after the 2 days have passed, you'll have to make another call to <code>GetSoftwareUpdates</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-get-software-updates-result-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: GetSoftwareUpdatesResult
---
