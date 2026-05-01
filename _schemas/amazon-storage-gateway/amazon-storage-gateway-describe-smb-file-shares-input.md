---
description: DescribeSMBFileSharesInput
layout: schema
name: DescribeSMBFileSharesInput
properties_list:
- description: ''
  name: FileShareARNList
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-smb-file-shares-input-schema.json
slug: amazon-storage-gateway-describe-smb-file-shares-input
source_filename: amazon-storage-gateway-describe-smb-file-shares-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-smb-file-shares-input-schema.json\",\n  \"title\": \"DescribeSMBFileSharesInput\",\n  \"description\": \"DescribeSMBFileSharesInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileShareARNList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileShareARNList\"\n        },\n        {\n          \"description\": \"An array containing the Amazon Resource Name (ARN) of each file share to be described.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FileShareARNList\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-smb-file-shares-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeSMBFileSharesInput
---
