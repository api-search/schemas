---
description: The refresh cache information for the file share or FSx file systems.
layout: schema
name: CacheAttributes
properties_list:
- description: ''
  name: CacheStaleTimeoutInSeconds
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-cache-attributes-schema.json
slug: amazon-storage-gateway-cache-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-cache-attributes-schema.json\",\n  \"title\": \"CacheAttributes\",\n  \"description\": \"The refresh cache information for the file share or FSx file systems.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CacheStaleTimeoutInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CacheStaleTimeoutInSeconds\"\n        },\n        {\n          \"description\": \"<p>Refreshes a file share's cache by using Time To Live (TTL). TTL is the length of time since the last refresh after which access to the directory would cause the file gateway to first refresh that directory's contents from the Amazon S3 bucket or Amazon FSx file system. The TTL duration is in seconds.</p> <p>Valid Values:0, 300 to 2,592,000 seconds (5 minutes to 30 days)</p>\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-cache-attributes-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: CacheAttributes
---
