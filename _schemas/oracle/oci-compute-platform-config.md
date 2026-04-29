---
description: The platform configuration for the instance. Includes settings for Secure Boot, measured boot, and trusted platform module.
layout: schema
name: PlatformConfig
properties_list:
- description: The type of platform configuration
  name: type
  type: string
- description: Whether Secure Boot is enabled on the instance
  name: isSecureBootEnabled
  type: boolean
- description: Whether the Trusted Platform Module (TPM) is enabled
  name: isTrustedPlatformModuleEnabled
  type: boolean
- description: Whether the Measured Boot feature is enabled
  name: isMeasuredBootEnabled
  type: boolean
- description: Whether AMD memory encryption is enabled
  name: isMemoryEncryptionEnabled
  type: boolean
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-platform-config-schema.json
slug: oci-compute-platform-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlatformConfig\",\n  \"type\": \"object\",\n  \"description\": \"The platform configuration for the instance. Includes settings for Secure Boot, measured boot, and trusted platform module.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of platform configuration\"\n    },\n    \"isSecureBootEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Secure Boot is enabled on the instance\"\n    },\n    \"isTrustedPlatformModuleEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the Trusted Platform Module (TPM) is enabled\"\n    },\n    \"isMeasuredBootEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the Measured Boot feature is enabled\"\n    },\n    \"isMemoryEncryptionEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether AMD memory encryption\
  \ is enabled\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-platform-config-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: PlatformConfig
---
