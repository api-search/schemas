---
description: The Subject Alternative Names of a X509 object.
layout: schema
name: SubjectAlternativeNames
properties_list:
- description: Email addresses.
  name: emails
  type: array
- description: Domain names.
  name: dns_names
  type: array
- description: User Principal Names.
  name: upns
  type: array
- description: Uniform Resource Identifiers.
  name: uris
  type: array
- description: IP addresses; supports IPv4 and IPv6.
  name: ipAddresses
  type: array
provider_name: Azure Key Vault
provider_slug: azure-key-vault
schema_file: json-schema/azure-key-vault-data-plane-subject-alternative-names-schema.json
slug: azure-key-vault-data-plane-subject-alternative-names
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubjectAlternativeNames\",\n  \"type\": \"object\",\n  \"description\": \"The Subject Alternative Names of a X509 object.\",\n  \"properties\": {\n    \"emails\": {\n      \"type\": \"array\",\n      \"description\": \"Email addresses.\"\n    },\n    \"dns_names\": {\n      \"type\": \"array\",\n      \"description\": \"Domain names.\"\n    },\n    \"upns\": {\n      \"type\": \"array\",\n      \"description\": \"User Principal Names.\"\n    },\n    \"uris\": {\n      \"type\": \"array\",\n      \"description\": \"Uniform Resource Identifiers.\"\n    },\n    \"ipAddresses\": {\n      \"type\": \"array\",\n      \"description\": \"IP addresses; supports IPv4 and IPv6.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-key-vault/refs/heads/main/json-schema/azure-key-vault-data-plane-subject-alternative-names-schema.json
tags:
- Certificates
- Cloud Security
- Cryptography
- Key Management
- Secrets Management
- Security
title: SubjectAlternativeNames
---
