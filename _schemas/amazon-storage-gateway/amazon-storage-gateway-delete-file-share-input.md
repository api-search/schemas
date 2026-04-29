---
description: DeleteFileShareInput
layout: schema
name: DeleteFileShareInput
properties_list:
- description: ''
  name: FileShareARN
  type: object
- description: ''
  name: ForceDelete
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-delete-file-share-input-schema.json
slug: amazon-storage-gateway-delete-file-share-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-file-share-input-schema.json\",\n  \"title\": \"DeleteFileShareInput\",\n  \"description\": \"DeleteFileShareInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileShareARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileShareARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the file share to be deleted.\"\n        }\n      ]\n    },\n    \"ForceDelete\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/boolean\"\n        },\n        {\n          \"description\": \"<p>If this value is set to <code>true</code>, the operation deletes a file share immediately and aborts all data uploads to Amazon Web Services. Otherwise, the file share is not deleted until\
  \ all data is uploaded to Amazon Web Services. This process aborts the data upload process, and the file share enters the <code>FORCE_DELETING</code> status.</p> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FileShareARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-file-share-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DeleteFileShareInput
---
