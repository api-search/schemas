---
description: Details for creating a preauthenticated request.
layout: schema
name: CreatePreauthenticatedRequestDetails
properties_list:
- description: A user-specified name for the pre-authenticated request.
  name: name
  type: string
- description: Name of object to grant access to. Omit for bucket-level access.
  name: objectName
  type: string
- description: The operation that can be performed.
  name: accessType
  type: string
- description: The expiration date for the pre-authenticated request.
  name: timeExpires
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/object-storage-create-preauthenticated-request-details-schema.json
slug: object-storage-create-preauthenticated-request-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/object-storage-create-preauthenticated-request-details-schema.json\",\n  \"title\": \"CreatePreauthenticatedRequestDetails\",\n  \"description\": \"Details for creating a preauthenticated request.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"accessType\",\n    \"timeExpires\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A user-specified name for the pre-authenticated request.\",\n      \"example\": \"my-par\"\n    },\n    \"objectName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of object to grant access to. Omit for bucket-level access.\",\n      \"example\": \"example-value\"\n    },\n    \"accessType\": {\n      \"type\": \"string\",\n      \"description\": \"The operation that can be performed.\",\n     \
  \ \"enum\": \"['ObjectRead', 'ObjectWrite', 'ObjectReadWrite', 'AnyObjectRead', 'AnyObjectWrite', 'AnyObjectReadWrite']\",\n      \"example\": \"ObjectRead\"\n    },\n    \"timeExpires\": {\n      \"type\": \"string\",\n      \"description\": \"The expiration date for the pre-authenticated request.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-12-31T23:59:59Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/object-storage-create-preauthenticated-request-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: CreatePreauthenticatedRequestDetails
---
