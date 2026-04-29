---
description: Represents a zone migration operation in Oracle Solaris, including migration type, state, progress tracking, connection details, and encryption cipher configuration for live and cold migrations between hosts.
layout: schema
name: Oracle Solaris Zone Migration
properties_list:
- description: Name of the zone being migrated
  name: zoneName
  type: string
- description: Destination host for the migration
  name: host
  type: string
- description: Migration type
  name: type
  type: string
- description: Current migration state
  name: state
  type: string
- description: Encryption cipher used for the migration data transfer
  name: cipher
  type:
  - string
  - 'null'
- description: ''
  name: progress
  type: object
- description: ''
  name: error
  type: object
- description: ''
  name: connection
  type: object
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-migration-schema.json
slug: solaris-zone-migration
source_filename: solaris-zone-migration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.oracle.com/schemas/solaris/zone-migration.json\",\n  \"title\": \"Oracle Solaris Zone Migration\",\n  \"description\": \"Represents a zone migration operation in Oracle Solaris, including migration type, state, progress tracking, connection details, and encryption cipher configuration for live and cold migrations between hosts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"zoneName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the zone being migrated\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Destination host for the migration\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Migration type\",\n      \"enum\": [\"live\", \"cold\"]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current migration state\",\n      \"enum\": [\"NONE\", \"INITIALIZED\"\
  , \"MIGRATING\", \"COMPLETED\"]\n    },\n    \"cipher\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Encryption cipher used for the migration data transfer\"\n    },\n    \"progress\": {\n      \"$ref\": \"#/$defs/MigrationProgress\"\n    },\n    \"error\": {\n      \"$ref\": \"#/$defs/MigrationError\"\n    },\n    \"connection\": {\n      \"$ref\": \"#/$defs/MigrationConnection\"\n    }\n  },\n  \"$defs\": {\n    \"MigrationProgress\": {\n      \"type\": \"object\",\n      \"description\": \"Progress information for an ongoing migration\",\n      \"properties\": {\n        \"zone\": {\n          \"type\": \"string\",\n          \"description\": \"Zone name\"\n        },\n        \"operation\": {\n          \"type\": \"string\",\n          \"description\": \"Current migration operation\",\n          \"enum\": [\n            \"FRAMEWORK\",\n            \"CONNECT\",\n            \"INIT_CRYPTO\",\n            \"CONFIG_CHECK\",\n            \"CONFIGURE\",\n       \
  \     \"ATTACH\",\n            \"BOOT\",\n            \"MIGRATE_INITIAL\",\n            \"MIGRATE\",\n            \"SUSPEND\",\n            \"RESTART\",\n            \"HALT\",\n            \"DETACH\",\n            \"UNCONFIGURE\",\n            \"COMPLETE\",\n            \"CANCEL\"\n          ]\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable progress message\"\n        },\n        \"percentComplete\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Progress percentage (0-100)\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        }\n      }\n    },\n    \"MigrationError\": {\n      \"type\": \"object\",\n      \"description\": \"Error information from a failed migration\",\n      \"properties\": {\n        \"operation\": {\n          \"type\": \"string\",\n          \"description\": \"The operation that failed\",\n          \"enum\": [\n            \"FRAMEWORK\",\n            \"CONNECT\"\
  ,\n            \"INIT_CRYPTO\",\n            \"CONFIG_CHECK\",\n            \"CONFIGURE\",\n            \"ATTACH\",\n            \"BOOT\",\n            \"MIGRATE_INITIAL\",\n            \"MIGRATE\",\n            \"SUSPEND\",\n            \"RESTART\",\n            \"HALT\",\n            \"DETACH\",\n            \"UNCONFIGURE\",\n            \"COMPLETE\",\n            \"CANCEL\"\n          ]\n        },\n        \"error\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"System or zone configuration error code\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable error message\"\n        }\n      }\n    },\n    \"MigrationConnection\": {\n      \"type\": \"object\",\n      \"description\": \"Remote host connection details for migration\",\n      \"properties\": {\n        \"hostname\": {\n          \"type\": \"string\",\n          \"description\": \"Remote host name or address\"\n        },\n      \
  \  \"supportsMultipleZones\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the remote host supports multi-zone migration\"\n        },\n        \"supportsSolarisZones\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the remote host supports native Solaris zones\"\n        },\n        \"supportsSolaris10Zones\": {\n          \"type\": [\"boolean\", \"null\"],\n          \"description\": \"Whether the remote host supports Solaris 10 branded zones\"\n        },\n        \"supportedCiphers\": {\n          \"$ref\": \"#/$defs/SupportedCiphers\"\n        }\n      }\n    },\n    \"SupportedCiphers\": {\n      \"type\": \"object\",\n      \"description\": \"Encryption ciphers supported for migration\",\n      \"properties\": {\n        \"source\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Ciphers supported by the source host\"\n        },\n    \
  \    \"destination\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Ciphers supported by the destination host\"\n        },\n        \"defaultCipher\": {\n          \"type\": \"string\",\n          \"description\": \"Default cipher for migration\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-migration-schema.json
tags:
- Containers
- Kernel Zones
- Operating Systems
- Oracle
- RAD
- Resource Management
- Solaris
- StatsStore
- Virtualization
- Zones
title: Oracle Solaris Zone Migration
---
