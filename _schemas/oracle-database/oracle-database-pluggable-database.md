---
description: Represents an Oracle Pluggable Database (PDB) in a multitenant container database architecture. PDBs are portable, self-contained database containers that share the resources of a container database (CDB).
layout: schema
name: Oracle Pluggable Database
properties_list:
- description: Name of the pluggable database
  name: pdb_name
  type: string
- description: Unique identifier for the PDB within the CDB
  name: pdb_id
  type: integer
- description: The OCID of the pluggable database (OCI managed)
  name: id
  type: string
- description: The OCID of the container database (OCI managed)
  name: containerDatabaseId
  type: string
- description: The OCID of the compartment (OCI managed)
  name: compartmentId
  type: string
- description: Current status of the PDB
  name: status
  type: string
- description: Current open mode of the PDB
  name: open_mode
  type: string
- description: OCI lifecycle state of the PDB
  name: lifecycleState
  type: string
- description: Total size of the PDB in bytes
  name: total_size
  type: integer
- description: Timestamp when the PDB was created
  name: creation_time
  type: string
- description: Creation timestamp (OCI format)
  name: timeCreated
  type: string
- description: Connection strings for the PDB
  name: connectionStrings
  type: object
- description: Free-form tags for resource categorization
  name: freeformTags
  type: object
- description: Defined tags for resource governance
  name: definedTags
  type: object
provider_name: Oracle Database
provider_slug: oracle-database
schema_file: json-schema/oracle-database-pluggable-database.json
slug: oracle-database-pluggable-database
source_filename: oracle-database-pluggable-database.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://oracle.com/schemas/database/pluggable-database.json\",\n  \"title\": \"Oracle Pluggable Database\",\n  \"description\": \"Represents an Oracle Pluggable Database (PDB) in a multitenant container database architecture. PDBs are portable, self-contained database containers that share the resources of a container database (CDB).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pdb_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the pluggable database\"\n    },\n    \"pdb_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the PDB within the CDB\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the pluggable database (OCI managed)\"\n    },\n    \"containerDatabaseId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the container database (OCI managed)\"\n    },\n\
  \    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the compartment (OCI managed)\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the PDB\",\n      \"enum\": [\"NORMAL\", \"RESTRICTED\", \"UNUSABLE\", \"RECOVERING\", \"NEW\"]\n    },\n    \"open_mode\": {\n      \"type\": \"string\",\n      \"description\": \"Current open mode of the PDB\",\n      \"enum\": [\"READ_WRITE\", \"READ_ONLY\", \"MOUNTED\", \"MIGRATE\"]\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"description\": \"OCI lifecycle state of the PDB\",\n      \"enum\": [\n        \"PROVISIONING\",\n        \"AVAILABLE\",\n        \"TERMINATING\",\n        \"TERMINATED\",\n        \"UPDATING\",\n        \"FAILED\"\n      ]\n    },\n    \"total_size\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Total size of the PDB in bytes\"\n    },\n    \"creation_time\": {\n    \
  \  \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the PDB was created\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp (OCI format)\"\n    },\n    \"connectionStrings\": {\n      \"type\": \"object\",\n      \"description\": \"Connection strings for the PDB\",\n      \"properties\": {\n        \"pdbDefault\": {\n          \"type\": \"string\",\n          \"description\": \"Default connection string for the PDB\"\n        },\n        \"pdbIpDefault\": {\n          \"type\": \"string\",\n          \"description\": \"IP-based default connection string for the PDB\"\n        }\n      }\n    },\n    \"freeformTags\": {\n      \"type\": \"object\",\n      \"description\": \"Free-form tags for resource categorization\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"definedTags\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"Defined tags for resource governance\",\n      \"additionalProperties\": {\n        \"type\": \"object\"\n      }\n    }\n  },\n  \"required\": [\"pdb_name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-database/refs/heads/main/json-schema/oracle-database-pluggable-database.json
tags:
- Cloud
- Database
- Enterprise
- Oracle
- REST API
- SQL
title: Oracle Pluggable Database
---
