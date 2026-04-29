---
description: Details for updating a bucket.
layout: schema
name: UpdateBucketDetails
properties_list:
- description: The name of the bucket.
  name: name
  type: string
- description: The Object Storage namespace.
  name: namespace
  type: string
- description: The OCID of the compartment.
  name: compartmentId
  type: string
- description: ''
  name: publicAccessType
  type: string
- description: ''
  name: objectEventsEnabled
  type: boolean
- description: ''
  name: versioning
  type: string
- description: ''
  name: freeformTags
  type: object
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/object-storage-update-bucket-details-schema.json
slug: object-storage-update-bucket-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/object-storage-update-bucket-details-schema.json\",\n  \"title\": \"UpdateBucketDetails\",\n  \"description\": \"Details for updating a bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the bucket.\",\n      \"example\": \"example-value\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The Object Storage namespace.\",\n      \"example\": \"oci_computeagent\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the compartment.\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"publicAccessType\": {\n      \"type\": \"string\",\n      \"enum\": \"['NoPublicAccess', 'ObjectRead', 'ObjectReadWithoutList']\"\
  ,\n      \"example\": \"NoPublicAccess\"\n    },\n    \"objectEventsEnabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"versioning\": {\n      \"type\": \"string\",\n      \"enum\": \"['Enabled', 'Suspended']\",\n      \"example\": \"Enabled\"\n    },\n    \"freeformTags\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key1\": \"value1\"\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/object-storage-update-bucket-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: UpdateBucketDetails
---
