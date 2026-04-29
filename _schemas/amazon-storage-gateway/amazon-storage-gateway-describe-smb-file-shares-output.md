---
description: DescribeSMBFileSharesOutput
layout: schema
name: DescribeSMBFileSharesOutput
properties_list:
- description: ''
  name: SMBFileShareInfoList
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-smb-file-shares-output-schema.json
slug: amazon-storage-gateway-describe-smb-file-shares-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-smb-file-shares-output-schema.json\",\n  \"title\": \"DescribeSMBFileSharesOutput\",\n  \"description\": \"DescribeSMBFileSharesOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SMBFileShareInfoList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SMBFileShareInfoList\"\n        },\n        {\n          \"description\": \"An array containing a description for each requested file share.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-smb-file-shares-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeSMBFileSharesOutput
---
