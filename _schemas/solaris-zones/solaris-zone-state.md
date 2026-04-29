---
description: Represents runtime state information for a Solaris zone as reported by zoneadm(8) and the RAD zonemgr module, including lifecycle state, resource utilization, and migration status.
layout: schema
name: Oracle Solaris Zone State
properties_list:
- description: Unique name identifying the zone on the system
  name: name
  type: string
- description: Kernel-assigned numeric zone ID, present only when the zone is running or ready
  name: id
  type: integer
- description: Universally unique identifier for the zone
  name: uuid
  type: string
- description: Current lifecycle state of the zone
  name: state
  type: string
- description: Zone brand type determining the runtime environment
  name: brand
  type: string
- description: Auxiliary state flags providing additional zone status information
  name: auxstate
  type: array
- description: Whether this is the global (host) zone
  name: isGlobal
  type: boolean
- description: File system path for the zone root
  name: zonepath
  type: string
- description: ''
  name: stateChange
  type: object
- description: ''
  name: migrationState
  type: object
- description: ''
  name: evacuationState
  type: object
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-state-schema.json
slug: solaris-zone-state
source_filename: solaris-zone-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.oracle.com/schemas/solaris/zone-state.json\",\n  \"title\": \"Oracle Solaris Zone State\",\n  \"description\": \"Represents runtime state information for a Solaris zone as reported by zoneadm(8) and the RAD zonemgr module, including lifecycle state, resource utilization, and migration status.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"state\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name identifying the zone on the system\",\n      \"minLength\": 1,\n      \"maxLength\": 64\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Kernel-assigned numeric zone ID, present only when the zone is running or ready\",\n      \"minimum\": -1\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Universally unique identifier for the zone\"\
  \n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle state of the zone\",\n      \"enum\": [\"configured\", \"incomplete\", \"installed\", \"ready\", \"running\", \"shutting_down\", \"down\"]\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Zone brand type determining the runtime environment\",\n      \"enum\": [\"solaris\", \"solaris10\", \"solaris-kz\", \"labeled\"]\n    },\n    \"auxstate\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Auxiliary state flags providing additional zone status information\"\n    },\n    \"isGlobal\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the global (host) zone\"\n    },\n    \"zonepath\": {\n      \"type\": \"string\",\n      \"description\": \"File system path for the zone root\"\n    },\n    \"stateChange\": {\n      \"$ref\": \"#/$defs/StateChange\"\n    },\n    \"migrationState\"\
  : {\n      \"$ref\": \"#/$defs/MigrationState\"\n    },\n    \"evacuationState\": {\n      \"$ref\": \"#/$defs/EvacuationState\"\n    }\n  },\n  \"$defs\": {\n    \"StateChange\": {\n      \"type\": \"object\",\n      \"description\": \"Record of a zone state transition event\",\n      \"properties\": {\n        \"zone\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the zone that changed state\"\n        },\n        \"oldState\": {\n          \"type\": \"string\",\n          \"description\": \"Previous zone state\",\n          \"enum\": [\"configured\", \"incomplete\", \"installed\", \"ready\", \"running\", \"shutting_down\", \"down\"]\n        },\n        \"newState\": {\n          \"type\": \"string\",\n          \"description\": \"New zone state\",\n          \"enum\": [\"configured\", \"incomplete\", \"installed\", \"ready\", \"running\", \"shutting_down\", \"down\"]\n        }\n      },\n      \"required\": [\"zone\", \"oldState\", \"newState\"]\n    },\n\
  \    \"MigrationState\": {\n      \"type\": \"object\",\n      \"description\": \"Current migration state for a zone being migrated between hosts\",\n      \"properties\": {\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"Migration lifecycle state\",\n          \"enum\": [\"none\", \"initialized\", \"migrating\", \"completed\"]\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Migration type\",\n          \"enum\": [\"live\", \"cold\"]\n        },\n        \"remoteHost\": {\n          \"type\": \"string\",\n          \"description\": \"Target or source host for the migration\"\n        },\n        \"progress\": {\n          \"$ref\": \"#/$defs/MigrationProgress\"\n        },\n        \"error\": {\n          \"$ref\": \"#/$defs/MigrationError\"\n        }\n      }\n    },\n    \"MigrationProgress\": {\n      \"type\": \"object\",\n      \"description\": \"Progress information for an in-flight zone migration\"\
  ,\n      \"properties\": {\n        \"zone\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the zone being migrated\"\n        },\n        \"operation\": {\n          \"type\": \"string\",\n          \"description\": \"Current migration operation phase\",\n          \"enum\": [\n            \"framework\",\n            \"connect\",\n            \"init_crypto\",\n            \"config_check\",\n            \"configure\",\n            \"attach\",\n            \"boot\",\n            \"migrate_initial\",\n            \"migrate\",\n            \"suspend\",\n            \"restart\",\n            \"halt\",\n            \"detach\",\n            \"unconfigure\",\n            \"complete\",\n            \"cancel\"\n          ]\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable progress message\"\n        },\n        \"percentComplete\": {\n          \"type\": \"integer\",\n          \"description\": \"Percentage\
  \ of migration completed\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        }\n      }\n    },\n    \"MigrationError\": {\n      \"type\": \"object\",\n      \"description\": \"Error information for a failed migration operation\",\n      \"properties\": {\n        \"operation\": {\n          \"type\": \"string\",\n          \"description\": \"The migration operation that failed\"\n        },\n        \"domain\": {\n          \"type\": \"string\",\n          \"description\": \"Error domain classification\",\n          \"enum\": [\"system\", \"zonecfg\"]\n        },\n        \"errno\": {\n          \"type\": \"integer\",\n          \"description\": \"System error number\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable error description\"\n        }\n      }\n    },\n    \"EvacuationState\": {\n      \"type\": \"object\",\n      \"description\": \"State information for a zone evacuation operation\",\n     \
  \ \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Overall evacuation status\",\n          \"enum\": [\"success\", \"fail\", \"partial_fail\"]\n        },\n        \"returning\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether zones are being returned from a previous evacuation\"\n        },\n        \"milestone\": {\n          \"type\": \"string\",\n          \"description\": \"Current evacuation milestone\",\n          \"enum\": [\n            \"migrate_initializing\",\n            \"migrate_initialization_complete\",\n            \"migrate_initialization_fail\",\n            \"migrating\",\n            \"migrate_complete\",\n            \"migrate_fail\",\n            \"evacuate_initializing\",\n            \"evacuate_initialization_complete\",\n            \"evacuate_initialization_fail\",\n            \"evacuating\",\n            \"evacuate_complete\",\n            \"evacuate_fail\",\n            \"evacuate_canceled\"\
  \n          ]\n        },\n        \"zoneCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of zones involved in the evacuation\",\n          \"minimum\": 0\n        },\n        \"transferRate\": {\n          \"type\": \"integer\",\n          \"description\": \"Current data transfer rate in bytes per second\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-state-schema.json
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
title: Oracle Solaris Zone State
---
