---
description: DescribeFileSystemAssociationsOutput schema from Amazon Storage Gateway API
layout: schema
name: DescribeFileSystemAssociationsOutput
properties_list:
- description: ''
  name: FileSystemAssociationInfoList
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-file-system-associations-output-schema.json
slug: amazon-storage-gateway-describe-file-system-associations-output
source_filename: amazon-storage-gateway-describe-file-system-associations-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-file-system-associations-output-schema.json\",\n  \"title\": \"DescribeFileSystemAssociationsOutput\",\n  \"description\": \"DescribeFileSystemAssociationsOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileSystemAssociationInfoList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSystemAssociationInfoList\"\n        },\n        {\n          \"description\": \"An array containing the <code>FileSystemAssociationInfo</code> data type of each file system association to be described. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-file-system-associations-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeFileSystemAssociationsOutput
---
