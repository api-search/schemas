---
description: Platform configuration options available for the shape
layout: schema
name: ShapePlatformConfigOptions
properties_list:
- description: The type of platform configuration
  name: type
  type: string
- description: Whether Secure Boot is supported
  name: isSecureBootEnabled
  type: boolean
- description: Whether the Trusted Platform Module is supported
  name: isTrustedPlatformModuleEnabled
  type: boolean
- description: Whether Measured Boot is supported
  name: isMeasuredBootEnabled
  type: boolean
- description: Whether memory encryption is supported
  name: isMemoryEncryptionEnabled
  type: boolean
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-shape-platform-config-options-schema.json
slug: oci-compute-shape-platform-config-options
source_filename: oci-compute-shape-platform-config-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ShapePlatformConfigOptions\",\n  \"type\": \"object\",\n  \"description\": \"Platform configuration options available for the shape\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of platform configuration\"\n    },\n    \"isSecureBootEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Secure Boot is supported\"\n    },\n    \"isTrustedPlatformModuleEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the Trusted Platform Module is supported\"\n    },\n    \"isMeasuredBootEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Measured Boot is supported\"\n    },\n    \"isMemoryEncryptionEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether memory encryption is supported\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-shape-platform-config-options-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: ShapePlatformConfigOptions
---
