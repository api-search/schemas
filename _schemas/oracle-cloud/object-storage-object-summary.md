---
description: Summary of an object in a bucket.
layout: schema
name: ObjectSummary
properties_list:
- description: The name of the object.
  name: name
  type: string
- description: Size of the object in bytes.
  name: size
  type: integer
- description: Base64-encoded MD5 hash.
  name: md5
  type: string
- description: The date and time the object was created.
  name: timeCreated
  type: string
- description: The date and time the object was last modified.
  name: timeModified
  type: string
- description: The storage tier of the object.
  name: storageTier
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/object-storage-object-summary-schema.json
slug: object-storage-object-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/object-storage-object-summary-schema.json\",\n  \"title\": \"ObjectSummary\",\n  \"description\": \"Summary of an object in a bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the object.\",\n      \"example\": \"documents/report.pdf\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"Size of the object in bytes.\",\n      \"example\": 1048576\n    },\n    \"md5\": {\n      \"type\": \"string\",\n      \"description\": \"Base64-encoded MD5 hash.\",\n      \"example\": \"aGVsbG93b3JsZA==\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the object was created.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\
  \n    },\n    \"timeModified\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the object was last modified.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    },\n    \"storageTier\": {\n      \"type\": \"string\",\n      \"description\": \"The storage tier of the object.\",\n      \"enum\": \"['Standard', 'InfrequentAccess', 'Archive']\",\n      \"example\": \"Standard\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/object-storage-object-summary-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: ObjectSummary
---
