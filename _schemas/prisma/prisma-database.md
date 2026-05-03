---
description: A Prisma Postgres database instance running PostgreSQL v17 on unikernel-based infrastructure. Includes built-in connection pooling, query caching via Accelerate, and real-time subscription capabilities via Pulse. Databases are provisioned within projects and can be managed through the Management API or the Prisma Console.
layout: schema
name: Prisma Postgres Database
properties_list:
- description: Unique identifier for the database
  name: id
  type: string
- description: Display name of the database
  name: name
  type: string
- description: Identifier of the parent project
  name: projectId
  type: string
- description: Cloud region where the database is deployed
  name: region
  type: string
- description: Current operational status of the database
  name: status
  type: string
- description: Database engine type
  name: engine
  type: string
- description: PostgreSQL version
  name: engineVersion
  type: string
- description: Prisma Postgres connection string in prisma+postgres:// format for use with Prisma Client
  name: connectionString
  type: string
- description: API keys for accessing the database through Prisma's connection pooler
  name: apiKeys
  type: array
- description: ''
  name: directConnection
  type: object
- description: ''
  name: usage
  type: object
- description: Available backups for the database
  name: backups
  type: array
- description: ISO 8601 timestamp when the database was created
  name: createdAt
  type: string
- description: ISO 8601 timestamp when the database was last updated
  name: updatedAt
  type: string
provider_name: Prisma
provider_slug: prisma
schema_file: json-schema/prisma-database-schema.json
slug: prisma-database
source_filename: prisma-database-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://prisma.io/schemas/database.json\",\n  \"title\": \"Prisma Postgres Database\",\n  \"description\": \"A Prisma Postgres database instance running PostgreSQL v17 on unikernel-based infrastructure. Includes built-in connection pooling, query caching via Accelerate, and real-time subscription capabilities via Pulse. Databases are provisioned within projects and can be managed through the Management API or the Prisma Console.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the database\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the database\",\n      \"examples\": [\"Production Database\"]\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the parent project\"\n    },\n    \"region\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Cloud region where the database is deployed\",\n      \"enum\": [\"us-east-1\", \"us-west-2\", \"eu-west-1\", \"eu-central-1\", \"ap-southeast-1\", \"ap-northeast-1\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational status of the database\",\n      \"enum\": [\"provisioning\", \"active\", \"suspended\", \"deleting\", \"deleted\"]\n    },\n    \"engine\": {\n      \"type\": \"string\",\n      \"description\": \"Database engine type\",\n      \"const\": \"postgresql\"\n    },\n    \"engineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"PostgreSQL version\",\n      \"examples\": [\"17\"]\n    },\n    \"connectionString\": {\n      \"type\": \"string\",\n      \"description\": \"Prisma Postgres connection string in prisma+postgres:// format for use with Prisma Client\",\n      \"examples\": [\"prisma+postgres://accelerate.prisma-data.net/?api_key=ey...\"]\n    },\n    \"apiKeys\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"API keys for accessing the database through Prisma's connection pooler\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ApiKey\"\n      }\n    },\n    \"directConnection\": {\n      \"$ref\": \"#/$defs/DirectConnection\"\n    },\n    \"usage\": {\n      \"$ref\": \"#/$defs/DatabaseUsage\"\n    },\n    \"backups\": {\n      \"type\": \"array\",\n      \"description\": \"Available backups for the database\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Backup\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the database was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the database was last updated\"\n    }\n  },\n  \"required\": [\"id\", \"projectId\", \"region\", \"status\", \"createdAt\", \"updatedAt\"],\n  \"additionalProperties\"\
  : false,\n  \"$defs\": {\n    \"ApiKey\": {\n      \"type\": \"object\",\n      \"description\": \"An API key for accessing the database through Prisma's infrastructure\",\n      \"properties\": {\n        \"apiKey\": {\n          \"type\": \"string\",\n          \"description\": \"The API key value\"\n        },\n        \"connectionString\": {\n          \"type\": \"string\",\n          \"description\": \"Full connection string incorporating this API key\"\n        }\n      },\n      \"required\": [\"apiKey\", \"connectionString\"]\n    },\n    \"DirectConnection\": {\n      \"type\": \"object\",\n      \"description\": \"Direct TCP connection details for connecting to the PostgreSQL instance without Prisma's proxy layer\",\n      \"properties\": {\n        \"host\": {\n          \"type\": \"string\",\n          \"description\": \"Database host address\"\n        },\n        \"port\": {\n          \"type\": \"integer\",\n          \"description\": \"Database port number\",\n        \
  \  \"default\": 5432\n        },\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"Database username\"\n        },\n        \"password\": {\n          \"type\": \"string\",\n          \"description\": \"Database password\"\n        },\n        \"database\": {\n          \"type\": \"string\",\n          \"description\": \"Database name\"\n        },\n        \"sslMode\": {\n          \"type\": \"string\",\n          \"description\": \"SSL connection mode\",\n          \"enum\": [\"require\", \"verify-ca\", \"verify-full\"],\n          \"default\": \"require\"\n        }\n      },\n      \"required\": [\"host\", \"port\", \"username\", \"password\", \"database\"]\n    },\n    \"DatabaseUsage\": {\n      \"type\": \"object\",\n      \"description\": \"Current usage metrics for the database\",\n      \"properties\": {\n        \"storageUsedBytes\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Total\
  \ storage consumed in bytes\"\n        },\n        \"storageLimitBytes\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Storage limit for the current plan in bytes\"\n        },\n        \"queryCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Total number of queries executed in the current billing period\"\n        },\n        \"connectionCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Current number of active connections\"\n        }\n      }\n    },\n    \"Backup\": {\n      \"type\": \"object\",\n      \"description\": \"A database backup snapshot\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the backup\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of backup\",\n          \"enum\": [\"automatic\", \"manual\"\
  ]\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Current status of the backup\",\n          \"enum\": [\"pending\", \"in_progress\", \"completed\", \"failed\"]\n        },\n        \"sizeBytes\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Size of the backup in bytes\"\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the backup was created\"\n        },\n        \"completedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the backup completed\"\n        }\n      },\n      \"required\": [\"id\", \"type\", \"status\", \"createdAt\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/prisma/refs/heads/main/json-schema/prisma-database-schema.json
tags: []
title: Prisma Postgres Database
---
