---
description: Summary of a preauthenticated request.
layout: schema
name: PreauthenticatedRequestSummary
properties_list:
- description: The unique identifier.
  name: id
  type: string
- description: The user-provided name.
  name: name
  type: string
- description: The name of the object.
  name: objectName
  type: string
- description: The operation that can be performed.
  name: accessType
  type: string
- description: The expiration date.
  name: timeExpires
  type: string
- description: ''
  name: timeCreated
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/object-storage-preauthenticated-request-summary-schema.json
slug: object-storage-preauthenticated-request-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/object-storage-preauthenticated-request-summary-schema.json\",\n  \"title\": \"PreauthenticatedRequestSummary\",\n  \"description\": \"Summary of a preauthenticated request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier.\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The user-provided name.\",\n      \"example\": \"example-value\"\n    },\n    \"objectName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the object.\",\n      \"example\": \"example-value\"\n    },\n    \"accessType\": {\n      \"type\": \"string\",\n      \"description\": \"The operation that can be performed.\",\n      \"enum\"\
  : \"['ObjectRead', 'ObjectWrite', 'ObjectReadWrite', 'AnyObjectRead', 'AnyObjectWrite', 'AnyObjectReadWrite']\",\n      \"example\": \"ObjectRead\"\n    },\n    \"timeExpires\": {\n      \"type\": \"string\",\n      \"description\": \"The expiration date.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/object-storage-preauthenticated-request-summary-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: PreauthenticatedRequestSummary
---
