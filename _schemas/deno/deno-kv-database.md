---
description: Represents a Deno KV database managed by Deno Deploy. Deno KV is a key-value database built into the Deno runtime and available as a globally distributed store on Deno Deploy. Locally it uses SQLite; on Deno Deploy data is replicated across regions. Databases are accessed from Deno code via Deno.openKv() using a KV Connect URL.
layout: schema
name: Deno KV Database
properties_list:
- description: Unique identifier for the KV database, used in the KV Connect URL
  name: databaseId
  type: string
- description: Optional human-readable description of the database's purpose or contents
  name: description
  type:
  - string
  - 'null'
- description: 'KV Connect URL used to open this database from Deno code: https://api.deno.com/databases/{database-id}/connect'
  name: kvConnect
  type: string
- description: UUID of the organization that owns this database
  name: organizationId
  type: string
- description: ISO 8601 UTC timestamp when the database was created
  name: createdAt
  type: string
- description: ISO 8601 UTC timestamp when the database was last modified
  name: updatedAt
  type: string
provider_name: Deno
provider_slug: deno
schema_file: json-schema/deno-kv-database-schema.json
slug: deno-kv-database
source_filename: deno-kv-database-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/deno/schemas/deno/kv-database.json\",\n  \"title\": \"Deno KV Database\",\n  \"description\": \"Represents a Deno KV database managed by Deno Deploy. Deno KV is a key-value database built into the Deno runtime and available as a globally distributed store on Deno Deploy. Locally it uses SQLite; on Deno Deploy data is replicated across regions. Databases are accessed from Deno code via Deno.openKv() using a KV Connect URL.\",\n  \"type\": \"object\",\n  \"required\": [\"databaseId\"],\n  \"properties\": {\n    \"databaseId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the KV database, used in the KV Connect URL\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Optional human-readable description of the database's purpose or contents\"\n    },\n  \
  \  \"kvConnect\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"KV Connect URL used to open this database from Deno code: https://api.deno.com/databases/{database-id}/connect\",\n      \"pattern\": \"^https://api\\\\.deno\\\\.com/databases/[0-9a-f-]+/connect$\"\n    },\n    \"organizationId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"UUID of the organization that owns this database\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 UTC timestamp when the database was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 UTC timestamp when the database was last modified\"\n    }\n  },\n  \"$defs\": {\n    \"KvKey\": {\n      \"type\": \"array\",\n      \"description\": \"A Deno KV key, which is an ordered tuple of key parts. Parts can be strings,\
  \ numbers, booleans, Uint8Arrays, or BigInts. Keys are lexicographically ordered, enabling hierarchical data modeling.\",\n      \"items\": {\n        \"description\": \"A single key part, which can be a string, number, boolean, or byte array\",\n        \"oneOf\": [\n          {\"type\": \"string\"},\n          {\"type\": \"number\"},\n          {\"type\": \"boolean\"}\n        ]\n      },\n      \"minItems\": 1\n    },\n    \"KvEntry\": {\n      \"type\": \"object\",\n      \"description\": \"A key-value entry in a Deno KV database, consisting of a key tuple, a value, and a versionstamp for optimistic concurrency control\",\n      \"required\": [\"key\", \"value\", \"versionstamp\"],\n      \"properties\": {\n        \"key\": {\n          \"$ref\": \"#/$defs/KvKey\"\n        },\n        \"value\": {\n          \"description\": \"The stored value, which can be any structured-serializable JavaScript value including objects, arrays, strings, numbers, booleans, Uint8Arrays, and Deno.KvU64\"\
  \n        },\n        \"versionstamp\": {\n          \"type\": \"string\",\n          \"description\": \"A monotonically increasing hex string representing the version of this entry, used for optimistic concurrency control in atomic operations\"\n        }\n      }\n    },\n    \"KvListSelector\": {\n      \"type\": \"object\",\n      \"description\": \"A selector for listing entries from a Deno KV database, supporting prefix-based and range-based queries\",\n      \"properties\": {\n        \"prefix\": {\n          \"$ref\": \"#/$defs/KvKey\",\n          \"description\": \"List all entries whose key starts with this prefix\"\n        },\n        \"start\": {\n          \"$ref\": \"#/$defs/KvKey\",\n          \"description\": \"List entries with keys greater than or equal to this key\"\n        },\n        \"end\": {\n          \"$ref\": \"#/$defs/KvKey\",\n          \"description\": \"List entries with keys less than this key\"\n        }\n      }\n    },\n    \"KvAtomicOperation\": {\n\
  \      \"type\": \"object\",\n      \"description\": \"An atomic operation on a Deno KV database, consisting of optional checks and mutations that are applied atomically. The operation succeeds only if all checks pass.\",\n      \"properties\": {\n        \"checks\": {\n          \"type\": \"array\",\n          \"description\": \"Preconditions that must all be satisfied for the operation to succeed. Each check verifies that a key's versionstamp matches an expected value.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/KvCheck\"\n          }\n        },\n        \"mutations\": {\n          \"type\": \"array\",\n          \"description\": \"Mutations to apply if all checks pass\",\n          \"items\": {\n            \"$ref\": \"#/$defs/KvMutation\"\n          }\n        }\n      }\n    },\n    \"KvCheck\": {\n      \"type\": \"object\",\n      \"description\": \"A precondition check for a Deno KV atomic operation, verifying that a key's current versionstamp matches an expected\
  \ value\",\n      \"required\": [\"key\"],\n      \"properties\": {\n        \"key\": {\n          \"$ref\": \"#/$defs/KvKey\"\n        },\n        \"versionstamp\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Expected versionstamp of the entry. Null means the entry must not exist.\"\n        }\n      }\n    },\n    \"KvMutation\": {\n      \"type\": \"object\",\n      \"description\": \"A single mutation to apply within a Deno KV atomic operation\",\n      \"required\": [\"type\", \"key\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of mutation to perform\",\n          \"enum\": [\"set\", \"delete\", \"sum\", \"max\", \"min\"]\n        },\n        \"key\": {\n          \"$ref\": \"#/$defs/KvKey\"\n        },\n        \"value\": {\n          \"description\": \"The value to set (for set/sum/max/min mutations)\"\n        },\n        \"expireIn\": {\n          \"type\": \"integer\"\
  ,\n          \"description\": \"Time-to-live in milliseconds for the entry (for set mutations)\",\n          \"minimum\": 1\n        }\n      }\n    },\n    \"KvDatabaseBackup\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for automatic S3 backup of a Deno KV database\",\n      \"required\": [\"id\", \"databaseId\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for the backup configuration\"\n        },\n        \"databaseId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"UUID of the KV database being backed up\"\n        },\n        \"bucketName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the S3 bucket where backups are stored\"\n        },\n        \"bucketRegion\": {\n          \"type\": \"string\",\n          \"description\": \"AWS region of the S3 bucket (e.g.,\
  \ us-east-1)\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Current status of the backup job\",\n          \"enum\": [\"pending\", \"active\", \"failed\", \"disabled\"]\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the backup was configured\"\n        },\n        \"updatedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the backup configuration was last modified\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/json-schema/deno-kv-database-schema.json
tags:
- Deployment
- Edge
- JavaScript
- Runtime
- Serverless
- TypeScript
title: Deno KV Database
---
