---
description: SaaSAccount schema from Incident Security Service Posture Management API
layout: schema
name: SaaSAccount
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: saasProviderId
  type: string
- description: ''
  name: tenant
  type: string
- description: ''
  name: saasInstanceId
  type: string
- description: ''
  name: jobId
  type: string
- description: ''
  name: appId
  type: string
- description: ''
  name: appType
  type: string
- description: ''
  name: accountType
  type: string
- description: ''
  name: accountName
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: isLocal
  type: boolean
- description: ''
  name: isOrphaned
  type: boolean
- description: ''
  name: isElevated
  type: boolean
- description: ''
  name: ticketKey
  type: string
- description: ''
  name: ticketUrl
  type: string
- description: ''
  name: roles
  type: string
- description: ''
  name: creator
  type: string
- description: ''
  name: linkedHumanAccounts
  type: string
- description: ''
  name: saasProviderNhiName
  type: string
- description: ''
  name: lastModifiedTime
  type: string
- description: ''
  name: lastLoginTime
  type: string
- description: ''
  name: isNonHuman
  type: boolean
- description: ''
  name: createdTime
  type: string
- description: ''
  name: latestScanTime
  type: string
- description: ''
  name: lastCredentialsRotated
  type: string
- description: ''
  name: rotatedBy
  type: string
- description: ''
  name: githubOrgName
  type: string
- description: ''
  name: credentialsExpiresAt
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/identity-security-posture-management-api-saa-s-account-schema.json
slug: identity-security-posture-management-api-saa-s-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SaaSAccount\",\n  \"description\": \"SaaSAccount schema from Incident Security Service Posture Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-saa-s-account-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"saasProviderId\": {\n      \"type\": \"string\"\n    },\n    \"tenant\": {\n      \"type\": \"string\"\n    },\n    \"saasInstanceId\": {\n      \"type\": \"string\"\n    },\n    \"jobId\": {\n      \"type\": \"string\"\n    },\n    \"appId\": {\n      \"type\": \"string\"\n    },\n    \"appType\": {\n      \"type\": \"string\"\n    },\n    \"accountType\": {\n      \"type\": \"string\"\n    },\n    \"accountName\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"type\": \"string\"\n \
  \   },\n    \"isLocal\": {\n      \"type\": \"boolean\"\n    },\n    \"isOrphaned\": {\n      \"type\": \"boolean\"\n    },\n    \"isElevated\": {\n      \"type\": \"boolean\"\n    },\n    \"ticketKey\": {\n      \"type\": \"string\"\n    },\n    \"ticketUrl\": {\n      \"type\": \"string\"\n    },\n    \"roles\": {\n      \"type\": \"string\"\n    },\n    \"creator\": {\n      \"type\": \"string\"\n    },\n    \"linkedHumanAccounts\": {\n      \"type\": \"string\"\n    },\n    \"saasProviderNhiName\": {\n      \"type\": \"string\"\n    },\n    \"lastModifiedTime\": {\n      \"format\": \"date-time\",\n      \"type\": \"string\",\n      \"example\": \"2022-03-10T16:15:50+00:00\"\n    },\n    \"lastLoginTime\": {\n      \"format\": \"date-time\",\n      \"type\": \"string\",\n      \"example\": \"2022-03-10T16:15:50+00:00\"\n    },\n    \"isNonHuman\": {\n      \"type\": \"boolean\"\n    },\n    \"createdTime\": {\n      \"format\": \"date-time\",\n      \"type\": \"string\",\n      \"\
  example\": \"2022-03-10T16:15:50+00:00\"\n    },\n    \"latestScanTime\": {\n      \"format\": \"date-time\",\n      \"type\": \"string\",\n      \"example\": \"2022-03-10T16:15:50+00:00\"\n    },\n    \"lastCredentialsRotated\": {\n      \"format\": \"date-time\",\n      \"type\": \"string\",\n      \"example\": \"2022-03-10T16:15:50+00:00\"\n    },\n    \"rotatedBy\": {\n      \"type\": \"string\"\n    },\n    \"githubOrgName\": {\n      \"type\": \"string\"\n    },\n    \"credentialsExpiresAt\": {\n      \"format\": \"date-time\",\n      \"type\": \"string\",\n      \"example\": \"2022-03-10T16:15:50+00:00\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/identity-security-posture-management-api-saa-s-account-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SaaSAccount
---
