---
description: Summary information about a bucket.
layout: schema
name: BucketSummary
properties_list:
- description: The Object Storage namespace.
  name: namespace
  type: string
- description: The name of the bucket.
  name: name
  type: string
- description: The OCID of the compartment.
  name: compartmentId
  type: string
- description: The OCID of the user who created the bucket.
  name: createdBy
  type: string
- description: The date and time the bucket was created.
  name: timeCreated
  type: string
- description: The entity tag (ETag) for the bucket.
  name: etag
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/object-storage-bucket-summary-schema.json
slug: object-storage-bucket-summary
source_filename: object-storage-bucket-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/object-storage-bucket-summary-schema.json\",\n  \"title\": \"BucketSummary\",\n  \"description\": \"Summary information about a bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The Object Storage namespace.\",\n      \"example\": \"my-namespace\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the bucket.\",\n      \"example\": \"my-bucket\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the compartment.\",\n      \"example\": \"ocid1.compartment.oc1..abcdefg123456\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the user who created the bucket.\",\n      \"example\": \"example-value\"\
  \n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the bucket was created.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The entity tag (ETag) for the bucket.\",\n      \"example\": \"example-value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/object-storage-bucket-summary-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: BucketSummary
---
