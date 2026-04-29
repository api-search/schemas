---
description: A rewrite response.
layout: schema
name: RewriteResponse
properties_list:
- description: The kind of item this is.
  name: kind
  type: string
- description: The total bytes rewritten so far.
  name: totalBytesRewritten
  type: string
- description: The total size of the object being copied.
  name: objectSize
  type: string
- description: Whether the rewrite is complete. If false, call the rewrite method again with the returned rewriteToken.
  name: done
  type: boolean
- description: A token to use in subsequent rewrite requests. Present only when the rewrite is not yet complete.
  name: rewriteToken
  type: string
provider_name: Google Cloud Storage
provider_slug: gcp-cloud-storage
schema_file: json-schema/gcp-cloud-storage-json-rewrite-response-schema.json
slug: gcp-cloud-storage-json-rewrite-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RewriteResponse\",\n  \"type\": \"object\",\n  \"description\": \"A rewrite response.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The kind of item this is.\"\n    },\n    \"totalBytesRewritten\": {\n      \"type\": \"string\",\n      \"description\": \"The total bytes rewritten so far.\"\n    },\n    \"objectSize\": {\n      \"type\": \"string\",\n      \"description\": \"The total size of the object being copied.\"\n    },\n    \"done\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the rewrite is complete. If false, call the rewrite method again with the returned rewriteToken.\"\n    },\n    \"rewriteToken\": {\n      \"type\": \"string\",\n      \"description\": \"A token to use in subsequent rewrite requests. Present only when the rewrite is not yet complete.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gcp-cloud-storage/refs/heads/main/json-schema/gcp-cloud-storage-json-rewrite-response-schema.json
tags:
- Archival
- Backup
- Blob Storage
- Cloud Storage
- Data
- File Storage
- Google Cloud
- Object Storage
- Storage
title: RewriteResponse
---
