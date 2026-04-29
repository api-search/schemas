---
description: An IAM user in Oracle Cloud Infrastructure.
layout: schema
name: User
properties_list:
- description: The OCID of the user.
  name: id
  type: string
- description: The OCID of the tenancy.
  name: compartmentId
  type: string
- description: The name of the user.
  name: name
  type: string
- description: The description of the user.
  name: description
  type: string
- description: The email address.
  name: email
  type: string
- description: ''
  name: lifecycleState
  type: string
- description: Whether MFA is activated.
  name: isMfaActivated
  type: boolean
- description: ''
  name: timeCreated
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/iam-user-schema.json
slug: iam-user
source_filename: iam-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/iam-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"An IAM user in Oracle Cloud Infrastructure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the user.\",\n      \"example\": \"ocid1.user.oc1..abcdefg123456\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the tenancy.\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the user.\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the user.\",\n      \"example\": \"John Smith\"\n    },\n    \"email\":\
  \ {\n      \"type\": \"string\",\n      \"description\": \"The email address.\",\n      \"format\": \"email\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"enum\": \"['CREATING', 'ACTIVE', 'INACTIVE', 'DELETING', 'DELETED']\",\n      \"example\": \"CREATING\"\n    },\n    \"isMfaActivated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether MFA is activated.\",\n      \"example\": true\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/iam-user-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: User
---
