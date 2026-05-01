---
description: Contains the details of an Amazon Neptune DB instance.
layout: schema
name: DBInstance
properties_list:
- description: The user-supplied database identifier.
  name: DBInstanceIdentifier
  type: string
- description: The compute and memory capacity of the instance.
  name: DBInstanceClass
  type: string
- description: The database engine (neptune).
  name: Engine
  type: string
- description: Current state of the instance.
  name: DBInstanceStatus
  type: string
- description: ''
  name: Endpoint
  type: object
- description: The cluster this instance belongs to.
  name: DBClusterIdentifier
  type: string
- description: The Availability Zone of the instance.
  name: AvailabilityZone
  type: string
- description: The weekly time range for system maintenance.
  name: PreferredMaintenanceWindow
  type: string
- description: The version of the database engine.
  name: EngineVersion
  type: string
- description: Whether minor version upgrades are applied automatically.
  name: AutoMinorVersionUpgrade
  type: boolean
- description: Whether the instance is publicly accessible.
  name: PubliclyAccessible
  type: boolean
- description: The ARN of the DB instance.
  name: DBInstanceArn
  type: string
- description: The failover priority for the instance.
  name: PromotionTier
  type: integer
- description: Whether the instance storage is encrypted.
  name: StorageEncrypted
  type: boolean
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/management-db-instance-schema.json
slug: management-db-instance
source_filename: management-db-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-db-instance-schema.json\",\n  \"title\": \"DBInstance\",\n  \"description\": \"Contains the details of an Amazon Neptune DB instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DBInstanceIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The user-supplied database identifier.\"\n    },\n    \"DBInstanceClass\": {\n      \"type\": \"string\",\n      \"description\": \"The compute and memory capacity of the instance.\"\n    },\n    \"Engine\": {\n      \"type\": \"string\",\n      \"description\": \"The database engine (neptune).\"\n    },\n    \"DBInstanceStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current state of the instance.\"\n    },\n    \"Endpoint\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Address\": {\n\
  \          \"type\": \"string\"\n        },\n        \"Port\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"DBClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The cluster this instance belongs to.\"\n    },\n    \"AvailabilityZone\": {\n      \"type\": \"string\",\n      \"description\": \"The Availability Zone of the instance.\"\n    },\n    \"PreferredMaintenanceWindow\": {\n      \"type\": \"string\",\n      \"description\": \"The weekly time range for system maintenance.\"\n    },\n    \"EngineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the database engine.\"\n    },\n    \"AutoMinorVersionUpgrade\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether minor version upgrades are applied automatically.\"\n    },\n    \"PubliclyAccessible\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the instance is publicly accessible.\"\n    },\n    \"DBInstanceArn\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The ARN of the DB instance.\"\n    },\n    \"PromotionTier\": {\n      \"type\": \"integer\",\n      \"description\": \"The failover priority for the instance.\"\n    },\n    \"StorageEncrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the instance storage is encrypted.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-db-instance-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: DBInstance
---
