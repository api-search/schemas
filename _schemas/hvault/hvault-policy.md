---
description: Represents an ACL policy in HashiCorp Vault that defines permissions for paths and operations.
layout: schema
name: Vault ACL Policy
properties_list:
- description: Name of the policy
  name: name
  type: string
- description: Policy document in HCL or JSON format defining path-based permissions
  name: policy
  type: string
provider_name: HashiCorp Vault
provider_slug: hvault
schema_file: json-schema/hvault-policy-schema.json
slug: hvault-policy
source_filename: hvault-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.hashicorp.com/schemas/vault/policy.json\",\n  \"title\": \"Vault ACL Policy\",\n  \"description\": \"Represents an ACL policy in HashiCorp Vault that defines permissions for paths and operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the policy\"\n    },\n    \"policy\": {\n      \"type\": \"string\",\n      \"description\": \"Policy document in HCL or JSON format defining path-based permissions\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hvault/refs/heads/main/json-schema/hvault-policy-schema.json
tags:
- Encryption
- Identity
- Infrastructure
- Secrets Management
- Security
title: Vault ACL Policy
---
