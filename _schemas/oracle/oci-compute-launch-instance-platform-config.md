---
description: The platform configuration for launching an instance
layout: schema
name: LaunchInstancePlatformConfig
properties_list:
- description: The type of platform configuration
  name: type
  type: string
- description: Whether Secure Boot is enabled
  name: isSecureBootEnabled
  type: boolean
- description: Whether the Trusted Platform Module is enabled
  name: isTrustedPlatformModuleEnabled
  type: boolean
- description: Whether Measured Boot is enabled
  name: isMeasuredBootEnabled
  type: boolean
- description: Whether AMD memory encryption is enabled
  name: isMemoryEncryptionEnabled
  type: boolean
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-launch-instance-platform-config-schema.json
slug: oci-compute-launch-instance-platform-config
source_filename: oci-compute-launch-instance-platform-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LaunchInstancePlatformConfig\",\n  \"type\": \"object\",\n  \"description\": \"The platform configuration for launching an instance\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of platform configuration\"\n    },\n    \"isSecureBootEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Secure Boot is enabled\"\n    },\n    \"isTrustedPlatformModuleEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the Trusted Platform Module is enabled\"\n    },\n    \"isMeasuredBootEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Measured Boot is enabled\"\n    },\n    \"isMemoryEncryptionEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether AMD memory encryption is enabled\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-launch-instance-platform-config-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: LaunchInstancePlatformConfig
---
