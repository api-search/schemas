---
description: Details for creating a new bucket.
layout: schema
name: CreateBucketDetails
properties_list:
- description: The name of the bucket.
  name: name
  type: string
- description: The OCID of the compartment.
  name: compartmentId
  type: string
- description: The public access type.
  name: publicAccessType
  type: string
- description: The storage tier type.
  name: storageTier
  type: string
- description: Whether events are emitted for object state changes.
  name: objectEventsEnabled
  type: boolean
- description: The versioning status.
  name: versioning
  type: string
- description: ''
  name: freeformTags
  type: object
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/object-storage-create-bucket-details-schema.json
slug: object-storage-create-bucket-details
source_filename: object-storage-create-bucket-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/object-storage-create-bucket-details-schema.json\",\n  \"title\": \"CreateBucketDetails\",\n  \"description\": \"Details for creating a new bucket.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"compartmentId\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the bucket.\",\n      \"example\": \"my-new-bucket\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the compartment.\",\n      \"example\": \"ocid1.compartment.oc1..abcdefg123456\"\n    },\n    \"publicAccessType\": {\n      \"type\": \"string\",\n      \"description\": \"The public access type.\",\n      \"enum\": \"['NoPublicAccess', 'ObjectRead', 'ObjectReadWithoutList']\",\n      \"example\": \"NoPublicAccess\"\
  ,\n      \"default\": \"NoPublicAccess\"\n    },\n    \"storageTier\": {\n      \"type\": \"string\",\n      \"description\": \"The storage tier type.\",\n      \"enum\": \"['Standard', 'Archive']\",\n      \"example\": \"Standard\",\n      \"default\": \"Standard\"\n    },\n    \"objectEventsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether events are emitted for object state changes.\",\n      \"example\": false,\n      \"default\": false\n    },\n    \"versioning\": {\n      \"type\": \"string\",\n      \"description\": \"The versioning status.\",\n      \"enum\": \"['Enabled', 'Disabled']\",\n      \"example\": \"Enabled\"\n    },\n    \"freeformTags\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key1\": \"value1\"\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/object-storage-create-bucket-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: CreateBucketDetails
---
