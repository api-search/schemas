---
description: <p>Contains information about storage volumes attached to MSK broker nodes.</p>
layout: schema
name: StorageInfo
properties_list:
- description: ''
  name: EbsStorageInfo
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-storage-info-schema.json
slug: msk-api-storage-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-storage-info-schema.json\",\n  \"title\": \"StorageInfo\",\n  \"description\": \"\\n            <p>Contains information about storage volumes attached to MSK broker nodes.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EbsStorageInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EBSStorageInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ebsStorageInfo\"\n          },\n          \"description\": \"\\n            <p>EBS volume information.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-storage-info-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: StorageInfo
---
