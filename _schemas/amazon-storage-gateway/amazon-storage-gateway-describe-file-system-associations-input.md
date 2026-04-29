---
description: DescribeFileSystemAssociationsInput schema from Amazon Storage Gateway API
layout: schema
name: DescribeFileSystemAssociationsInput
properties_list:
- description: ''
  name: FileSystemAssociationARNList
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-file-system-associations-input-schema.json
slug: amazon-storage-gateway-describe-file-system-associations-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-file-system-associations-input-schema.json\",\n  \"title\": \"DescribeFileSystemAssociationsInput\",\n  \"description\": \"DescribeFileSystemAssociationsInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileSystemAssociationARNList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSystemAssociationARNList\"\n        },\n        {\n          \"description\": \"An array containing the Amazon Resource Name (ARN) of each file system association to be described.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FileSystemAssociationARNList\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-file-system-associations-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeFileSystemAssociationsInput
---
