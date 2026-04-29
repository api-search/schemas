---
description: DescribeNFSFileSharesOutput
layout: schema
name: DescribeNFSFileSharesOutput
properties_list:
- description: ''
  name: NFSFileShareInfoList
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-nfs-file-shares-output-schema.json
slug: amazon-storage-gateway-describe-nfs-file-shares-output
source_filename: amazon-storage-gateway-describe-nfs-file-shares-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-nfs-file-shares-output-schema.json\",\n  \"title\": \"DescribeNFSFileSharesOutput\",\n  \"description\": \"DescribeNFSFileSharesOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NFSFileShareInfoList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NFSFileShareInfoList\"\n        },\n        {\n          \"description\": \"An array containing a description for each requested file share.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-nfs-file-shares-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeNFSFileSharesOutput
---
