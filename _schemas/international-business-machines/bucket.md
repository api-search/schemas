---
description: An IBM Cloud Object Storage bucket.
layout: schema
name: Cloud Object Storage Bucket
properties_list:
- description: The name of the bucket.
  name: name
  type: string
- description: The date the bucket was created.
  name: creation_date
  type: string
- description: The location constraint (e.g., us-south-standard).
  name: location_constraint
  type: string
- description: The storage class.
  name: storage_class
  type: string
- description: The service instance ID that owns this bucket.
  name: ibm_service_instance_id
  type: string
provider_name: International Business Machines
provider_slug: international-business-machines
schema_file: json-schema/bucket.json
slug: bucket
source_filename: bucket.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"bucket.json\",\n  \"title\": \"Cloud Object Storage Bucket\",\n  \"description\": \"An IBM Cloud Object Storage bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the bucket.\"\n    },\n    \"creation_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date the bucket was created.\"\n    },\n    \"location_constraint\": {\n      \"type\": \"string\",\n      \"description\": \"The location constraint (e.g., us-south-standard).\"\n    },\n    \"storage_class\": {\n      \"type\": \"string\",\n      \"description\": \"The storage class.\",\n      \"enum\": [\"standard\", \"vault\", \"cold\", \"smart\"]\n    },\n    \"ibm_service_instance_id\": {\n      \"type\": \"string\",\n      \"description\": \"The service instance ID that owns this bucket.\"\n    }\n \
  \ },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/json-schema/bucket.json
tags:
- Artificial Intelligence
- Cloud
- Enterprise
- IBM
title: Cloud Object Storage Bucket
---
