---
description: An IAM policy for a Cloud Storage resource.
layout: schema
name: Policy
properties_list:
- description: The kind of item this is.
  name: kind
  type: string
- description: The ID of the resource to which this policy belongs.
  name: resourceId
  type: string
- description: The version of the policy. Valid values are 1 and 3. Any request that specifies conditional role bindings must specify version 3.
  name: version
  type: integer
- description: HTTP 1.1 Entity tag for the policy. Used for optimistic concurrency control.
  name: etag
  type: string
- description: A list of members bound to a role.
  name: bindings
  type: array
provider_name: Google Cloud Storage
provider_slug: gcp-cloud-storage
schema_file: json-schema/gcp-cloud-storage-json-policy-schema.json
slug: gcp-cloud-storage-json-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Policy\",\n  \"type\": \"object\",\n  \"description\": \"An IAM policy for a Cloud Storage resource.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The kind of item this is.\"\n    },\n    \"resourceId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the resource to which this policy belongs.\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"The version of the policy. Valid values are 1 and 3. Any request that specifies conditional role bindings must specify version 3.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"HTTP 1.1 Entity tag for the policy. Used for optimistic concurrency control.\"\n    },\n    \"bindings\": {\n      \"type\": \"array\",\n      \"description\": \"A list of members bound to a role.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gcp-cloud-storage/refs/heads/main/json-schema/gcp-cloud-storage-json-policy-schema.json
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
title: Policy
---
