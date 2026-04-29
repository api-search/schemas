---
description: Options for tuning the compatibility and performance of VM shapes
layout: schema
name: LaunchOptions
properties_list:
- description: Emulation type for the boot volume. PARAVIRTUALIZED is recommended for best performance.
  name: bootVolumeType
  type: string
- description: Firmware used to boot the VM
  name: firmware
  type: string
- description: Emulation type for the physical network interface card (NIC). PARAVIRTUALIZED or VFIO is recommended.
  name: networkType
  type: string
- description: Emulation type for attached block volume data disks
  name: remoteDataVolumeType
  type: string
- description: Whether to enable in-transit encryption for the data volume's paravirtualized attachment
  name: isPvEncryptionInTransitEnabled
  type: boolean
- description: Whether to enable consistent volume naming
  name: isConsistentVolumeNamingEnabled
  type: boolean
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-launch-options-schema.json
slug: oci-compute-launch-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LaunchOptions\",\n  \"type\": \"object\",\n  \"description\": \"Options for tuning the compatibility and performance of VM shapes\",\n  \"properties\": {\n    \"bootVolumeType\": {\n      \"type\": \"string\",\n      \"description\": \"Emulation type for the boot volume. PARAVIRTUALIZED is recommended for best performance.\"\n    },\n    \"firmware\": {\n      \"type\": \"string\",\n      \"description\": \"Firmware used to boot the VM\"\n    },\n    \"networkType\": {\n      \"type\": \"string\",\n      \"description\": \"Emulation type for the physical network interface card (NIC). PARAVIRTUALIZED or VFIO is recommended.\"\n    },\n    \"remoteDataVolumeType\": {\n      \"type\": \"string\",\n      \"description\": \"Emulation type for attached block volume data disks\"\n    },\n    \"isPvEncryptionInTransitEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable\
  \ in-transit encryption for the data volume's paravirtualized attachment\"\n    },\n    \"isConsistentVolumeNamingEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable consistent volume naming\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-launch-options-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: LaunchOptions
---
