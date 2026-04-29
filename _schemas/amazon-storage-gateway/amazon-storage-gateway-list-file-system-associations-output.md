---
description: ListFileSystemAssociationsOutput schema from Amazon Storage Gateway API
layout: schema
name: ListFileSystemAssociationsOutput
properties_list:
- description: ''
  name: Marker
  type: object
- description: ''
  name: NextMarker
  type: object
- description: ''
  name: FileSystemAssociationSummaryList
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-list-file-system-associations-output-schema.json
slug: amazon-storage-gateway-list-file-system-associations-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-file-system-associations-output-schema.json\",\n  \"title\": \"ListFileSystemAssociationsOutput\",\n  \"description\": \"ListFileSystemAssociationsOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Marker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"If the request includes <code>Marker</code>, the response returns that value in this field.\"\n        }\n      ]\n    },\n    \"NextMarker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"If a value is present, there are more file system associations to return. In a subsequent request,\
  \ use <code>NextMarker</code> as the value for <code>Marker</code> to retrieve the next set of file system associations.\"\n        }\n      ]\n    },\n    \"FileSystemAssociationSummaryList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileSystemAssociationSummaryList\"\n        },\n        {\n          \"description\": \"An array of information about the Amazon FSx gateway's file system associations.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-file-system-associations-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ListFileSystemAssociationsOutput
---
