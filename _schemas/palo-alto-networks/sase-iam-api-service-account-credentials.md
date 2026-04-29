---
description: ServiceAccountCredentials schema from Palo Alto Networks SASE IAM Service API
layout: schema
name: ServiceAccountCredentials
properties_list:
- description: Unique identifier of the generated key.
  name: key_id
  type: string
- description: OAuth 2.0 client ID for this credential set.
  name: client_id
  type: string
- description: OAuth 2.0 client secret. Returned only once at creation time. Store this value securely as it cannot be retrieved again.
  name: client_secret
  type: string
- description: Description provided when the key was created.
  name: description
  type: string
- description: Expiration timestamp, or null if credentials do not expire.
  name: expires_at
  type: string
- description: ''
  name: created_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-iam-api-service-account-credentials-schema.json
slug: sase-iam-api-service-account-credentials
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceAccountCredentials\",\n  \"description\": \"ServiceAccountCredentials schema from Palo Alto Networks SASE IAM Service API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-iam-api-service-account-credentials-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the generated key.\"\n    },\n    \"client_id\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth 2.0 client ID for this credential set.\"\n    },\n    \"client_secret\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth 2.0 client secret. Returned only once at creation time. Store this value securely as it cannot be retrieved again.\",\n      \"writeOnly\": true\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Description provided when the key was created.\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Expiration timestamp, or null if credentials do not expire.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-iam-api-service-account-credentials-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ServiceAccountCredentials
---
