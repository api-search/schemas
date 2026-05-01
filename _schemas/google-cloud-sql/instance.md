---
description: A Cloud SQL database instance resource representing a managed MySQL, PostgreSQL, or SQL Server instance.
layout: schema
name: Google Cloud SQL Database Instance
properties_list:
- description: This is always sql#instance.
  name: kind
  type: string
- description: Name of the Cloud SQL instance.
  name: name
  type: string
- description: The project ID of the project containing the Cloud SQL instance.
  name: project
  type: string
- description: The current serving state of the Cloud SQL instance.
  name: state
  type: string
- description: The geographical region (e.g., us-central1, europe-west1).
  name: region
  type: string
- description: The database engine type and version.
  name: databaseVersion
  type: string
- description: ''
  name: settings
  type: object
- description: Connection name of the Cloud SQL instance used in connection strings.
  name: connectionName
  type: string
- description: ''
  name: ipAddresses
  type: array
- description: The time the instance was created.
  name: createTime
  type: string
- description: ''
  name: backendType
  type: string
- description: ''
  name: selfLink
  type: string
- description: ''
  name: serviceAccountEmailAddress
  type: string
provider_name: Google Cloud SQL
provider_slug: google-cloud-sql
schema_file: json-schema/instance-schema.json
slug: instance
source_filename: instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-sql/refs/heads/main/json-schema/instance-schema.json\",\n  \"title\": \"Google Cloud SQL Database Instance\",\n  \"description\": \"A Cloud SQL database instance resource representing a managed MySQL, PostgreSQL, or SQL Server instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"const\": \"sql#instance\",\n      \"description\": \"This is always sql#instance.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Cloud SQL instance.\",\n      \"pattern\": \"^[a-z][a-z0-9-]*[a-z0-9]$\",\n      \"maxLength\": 98\n    },\n    \"project\": {\n      \"type\": \"string\",\n      \"description\": \"The project ID of the project containing the Cloud SQL instance.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"SQL_INSTANCE_STATE_UNSPECIFIED\"\
  , \"RUNNABLE\", \"SUSPENDED\", \"PENDING_DELETE\", \"PENDING_CREATE\", \"MAINTENANCE\", \"FAILED\"],\n      \"description\": \"The current serving state of the Cloud SQL instance.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The geographical region (e.g., us-central1, europe-west1).\"\n    },\n    \"databaseVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The database engine type and version.\",\n      \"examples\": [\"MYSQL_8_0\", \"POSTGRES_15\", \"SQLSERVER_2019_STANDARD\"]\n    },\n    \"settings\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"tier\": {\n          \"type\": \"string\",\n          \"description\": \"The tier (machine type) for this instance.\"\n        },\n        \"edition\": {\n          \"type\": \"string\",\n          \"enum\": [\"EDITION_UNSPECIFIED\", \"ENTERPRISE\", \"ENTERPRISE_PLUS\"]\n        },\n        \"availabilityType\": {\n          \"type\": \"string\",\n          \"enum\"\
  : [\"SQL_AVAILABILITY_TYPE_UNSPECIFIED\", \"ZONAL\", \"REGIONAL\"]\n        },\n        \"dataDiskSizeGb\": {\n          \"type\": \"string\",\n          \"description\": \"The size of data disk in GB.\"\n        },\n        \"dataDiskType\": {\n          \"type\": \"string\",\n          \"enum\": [\"SQL_DATA_DISK_TYPE_UNSPECIFIED\", \"PD_SSD\", \"PD_HDD\"]\n        },\n        \"backupConfiguration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"enabled\": { \"type\": \"boolean\" },\n            \"startTime\": { \"type\": \"string\" },\n            \"binaryLogEnabled\": { \"type\": \"boolean\" }\n          }\n        },\n        \"ipConfiguration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"ipv4Enabled\": { \"type\": \"boolean\" },\n            \"requireSsl\": { \"type\": \"boolean\" },\n            \"privateNetwork\": { \"type\": \"string\" }\n          }\n        },\n        \"activationPolicy\": {\n          \"\
  type\": \"string\",\n          \"enum\": [\"SQL_ACTIVATION_POLICY_UNSPECIFIED\", \"ALWAYS\", \"NEVER\"]\n        }\n      }\n    },\n    \"connectionName\": {\n      \"type\": \"string\",\n      \"description\": \"Connection name of the Cloud SQL instance used in connection strings.\"\n    },\n    \"ipAddresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\"PRIMARY\", \"OUTGOING\", \"PRIVATE\"]\n          },\n          \"ipAddress\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the instance was created.\"\n    },\n    \"backendType\": {\n      \"type\": \"string\",\n      \"enum\": [\"SQL_BACKEND_TYPE_UNSPECIFIED\", \"FIRST_GEN\", \"SECOND_GEN\", \"EXTERNAL\"]\n    },\n    \"selfLink\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"serviceAccountEmailAddress\": {\n      \"type\": \"string\",\n      \"format\": \"email\"\n    }\n  },\n  \"required\": [\"name\", \"databaseVersion\", \"settings\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-sql/refs/heads/main/json-schema/instance-schema.json
tags:
- Database
- Google Cloud
- MySQL
- PostgreSQL
- Relational
- SQL
title: Google Cloud SQL Database Instance
---
