---
description: A bucket is a container for storing objects in Object Storage.
layout: schema
name: Bucket
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
- description: The type of public access enabled on this bucket.
  name: publicAccessType
  type: string
- description: The storage tier type.
  name: storageTier
  type: string
- description: Whether events are emitted for object state changes.
  name: objectEventsEnabled
  type: boolean
- description: ''
  name: freeformTags
  type: object
- description: ''
  name: definedTags
  type: object
- description: The entity tag for the object lifecycle policy.
  name: objectLifecyclePolicyEtag
  type: string
- description: Approximate number of objects in the bucket.
  name: approximateCount
  type: integer
- description: Approximate total size in bytes.
  name: approximateSize
  type: integer
- description: The versioning status of the bucket.
  name: versioning
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/object-storage-bucket-schema.json
slug: object-storage-bucket
source_filename: object-storage-bucket-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/object-storage-bucket-schema.json\",\n  \"title\": \"Bucket\",\n  \"description\": \"A bucket is a container for storing objects in Object Storage.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The Object Storage namespace.\",\n      \"example\": \"my-namespace\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the bucket.\",\n      \"example\": \"my-bucket\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the compartment.\",\n      \"example\": \"ocid1.compartment.oc1..abcdefg123456\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the user who created the bucket.\",\n      \"example\"\
  : \"example-value\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the bucket was created.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    },\n    \"publicAccessType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of public access enabled on this bucket.\",\n      \"enum\": \"['NoPublicAccess', 'ObjectRead', 'ObjectReadWithoutList']\",\n      \"example\": \"NoPublicAccess\"\n    },\n    \"storageTier\": {\n      \"type\": \"string\",\n      \"description\": \"The storage tier type.\",\n      \"enum\": \"['Standard', 'Archive']\",\n      \"example\": \"Standard\"\n    },\n    \"objectEventsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether events are emitted for object state changes.\",\n      \"example\": false\n    },\n    \"freeformTags\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key1\": \"value1\"\n      },\n      \"additionalProperties\"\
  : {\n        \"type\": \"string\"\n      }\n    },\n    \"definedTags\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key1\": \"value1\"\n      },\n      \"additionalProperties\": {\n        \"type\": \"object\"\n      }\n    },\n    \"objectLifecyclePolicyEtag\": {\n      \"type\": \"string\",\n      \"description\": \"The entity tag for the object lifecycle policy.\",\n      \"example\": \"example-value\"\n    },\n    \"approximateCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Approximate number of objects in the bucket.\",\n      \"example\": 1500\n    },\n    \"approximateSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Approximate total size in bytes.\",\n      \"example\": 1073741824\n    },\n    \"versioning\": {\n      \"type\": \"string\",\n      \"description\": \"The versioning status of the bucket.\",\n      \"enum\": \"['Enabled', 'Suspended', 'Disabled']\",\n      \"example\": \"Enabled\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/object-storage-bucket-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: Bucket
---
