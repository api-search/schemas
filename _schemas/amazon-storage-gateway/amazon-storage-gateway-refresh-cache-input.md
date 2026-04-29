---
description: RefreshCacheInput
layout: schema
name: RefreshCacheInput
properties_list:
- description: ''
  name: FileShareARN
  type: object
- description: ''
  name: FolderList
  type: object
- description: ''
  name: Recursive
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-refresh-cache-input-schema.json
slug: amazon-storage-gateway-refresh-cache-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-refresh-cache-input-schema.json\",\n  \"title\": \"RefreshCacheInput\",\n  \"description\": \"RefreshCacheInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileShareARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileShareARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the file share you want to refresh.\"\n        }\n      ]\n    },\n    \"FolderList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FolderList\"\n        },\n        {\n          \"description\": \"A comma-separated list of the paths of folders to refresh in the cache. The default is [<code>\\\"/\\\"</code>]. The default refreshes objects and folders at the root of the Amazon S3 bucket.\
  \ If <code>Recursive</code> is set to <code>true</code>, the entire S3 bucket that the file share has access to is refreshed.\"\n        }\n      ]\n    },\n    \"Recursive\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>A value that specifies whether to recursively refresh folders in the cache. The refresh includes folders that were in the cache the last time the gateway listed the folder's contents. If this value set to <code>true</code>, each folder that is listed in <code>FolderList</code> is recursively updated. Otherwise, subfolders listed in <code>FolderList</code> are not refreshed. Only objects that are in folders listed directly under <code>FolderList</code> are found and used for the update. The default is <code>true</code>.</p> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FileShareARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-refresh-cache-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: RefreshCacheInput
---
