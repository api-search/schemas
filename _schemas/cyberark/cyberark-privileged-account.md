---
description: A privileged account stored in the CyberArk Vault (PAM Self-Hosted or Privilege Cloud).
layout: schema
name: PrivilegedAccount
properties_list:
- description: ''
  name: id
  type: string
- description: Account display name.
  name: name
  type: string
- description: Hostname, FQDN, or IP of the target system.
  name: address
  type: string
- description: ''
  name: userName
  type: string
- description: Platform configuration controlling rotation policy.
  name: platformId
  type: string
- description: ''
  name: safeName
  type: string
- description: ''
  name: secretType
  type: string
- description: ''
  name: secretManagement
  type: object
- description: ''
  name: remoteMachinesAccess
  type: object
provider_name: CyberArk
provider_slug: cyberark
schema_file: json-schema/cyberark-privileged-account-schema.json
slug: cyberark-privileged-account
source_filename: cyberark-privileged-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cyberark/refs/heads/main/json-schema/cyberark-privileged-account-schema.json\",\n  \"title\": \"PrivilegedAccount\",\n  \"description\": \"A privileged account stored in the CyberArk Vault (PAM Self-Hosted or Privilege Cloud).\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"platformId\", \"safeName\"],\n  \"properties\": {\n    \"id\": { \"type\": \"string\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Account display name.\" },\n    \"address\": { \"type\": \"string\", \"description\": \"Hostname, FQDN, or IP of the target system.\" },\n    \"userName\": { \"type\": \"string\" },\n    \"platformId\": { \"type\": \"string\", \"description\": \"Platform configuration controlling rotation policy.\" },\n    \"safeName\": { \"type\": \"string\" },\n    \"secretType\": {\n      \"type\": \"string\",\n      \"enum\": [\"password\"\
  , \"key\", \"certificate\"]\n    },\n    \"secretManagement\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"automaticManagementEnabled\": { \"type\": \"boolean\" },\n        \"manualManagementReason\": { \"type\": \"string\" },\n        \"lastModifiedTime\": { \"type\": \"string\", \"format\": \"date-time\" }\n      }\n    },\n    \"remoteMachinesAccess\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"remoteMachines\": { \"type\": \"string\" },\n        \"accessRestrictedToRemoteMachines\": { \"type\": \"boolean\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cyberark/refs/heads/main/json-schema/cyberark-privileged-account-schema.json
tags:
- Authentication
- Cloud Security
- Conjur
- Credential Vault
- DevOps Secrets
- Endpoint Privilege Management
- Identity Security
- Machine Identity
- MFA
- OpenAPI
- PAM
- Privileged Access
- Privileged Access Management
- Secrets Management
- Session Management
- SSO
- Vault
- Zero Trust
title: PrivilegedAccount
---
