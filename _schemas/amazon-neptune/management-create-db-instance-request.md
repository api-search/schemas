---
description: CreateDBInstanceRequest schema from Neptune
layout: schema
name: CreateDBInstanceRequest
properties_list:
- description: The DB instance identifier.
  name: DBInstanceIdentifier
  type: string
- description: The compute and memory capacity of the instance.
  name: DBInstanceClass
  type: string
- description: The database engine to use (neptune).
  name: Engine
  type: string
- description: The identifier of the DB cluster to add the instance to.
  name: DBClusterIdentifier
  type: string
- description: The Availability Zone for the instance.
  name: AvailabilityZone
  type: string
- description: ''
  name: PreferredMaintenanceWindow
  type: string
- description: ''
  name: AutoMinorVersionUpgrade
  type: boolean
- description: Failover priority (0-15).
  name: PromotionTier
  type: integer
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/management-create-db-instance-request-schema.json
slug: management-create-db-instance-request
source_filename: management-create-db-instance-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-create-db-instance-request-schema.json\",\n  \"title\": \"CreateDBInstanceRequest\",\n  \"description\": \"CreateDBInstanceRequest schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DBInstanceIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The DB instance identifier.\"\n    },\n    \"DBInstanceClass\": {\n      \"type\": \"string\",\n      \"description\": \"The compute and memory capacity of the instance.\"\n    },\n    \"Engine\": {\n      \"type\": \"string\",\n      \"description\": \"The database engine to use (neptune).\",\n      \"default\": \"neptune\"\n    },\n    \"DBClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the DB cluster to add the instance to.\"\n    },\n    \"AvailabilityZone\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The Availability Zone for the instance.\"\n    },\n    \"PreferredMaintenanceWindow\": {\n      \"type\": \"string\"\n    },\n    \"AutoMinorVersionUpgrade\": {\n      \"type\": \"boolean\"\n    },\n    \"PromotionTier\": {\n      \"type\": \"integer\",\n      \"description\": \"Failover priority (0-15).\",\n      \"minimum\": 0,\n      \"maximum\": 15\n    }\n  },\n  \"required\": [\n    \"DBInstanceIdentifier\",\n    \"DBInstanceClass\",\n    \"Engine\",\n    \"DBClusterIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-create-db-instance-request-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: CreateDBInstanceRequest
---
