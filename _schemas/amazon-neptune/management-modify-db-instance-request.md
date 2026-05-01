---
description: ModifyDBInstanceRequest schema from Neptune
layout: schema
name: ModifyDBInstanceRequest
properties_list:
- description: The DB instance identifier.
  name: DBInstanceIdentifier
  type: string
- description: The new compute and memory capacity.
  name: DBInstanceClass
  type: string
- description: ''
  name: PreferredMaintenanceWindow
  type: string
- description: ''
  name: AutoMinorVersionUpgrade
  type: boolean
- description: ''
  name: NewDBInstanceIdentifier
  type: string
- description: ''
  name: PromotionTier
  type: integer
- description: ''
  name: ApplyImmediately
  type: boolean
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/management-modify-db-instance-request-schema.json
slug: management-modify-db-instance-request
source_filename: management-modify-db-instance-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-modify-db-instance-request-schema.json\",\n  \"title\": \"ModifyDBInstanceRequest\",\n  \"description\": \"ModifyDBInstanceRequest schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DBInstanceIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The DB instance identifier.\"\n    },\n    \"DBInstanceClass\": {\n      \"type\": \"string\",\n      \"description\": \"The new compute and memory capacity.\"\n    },\n    \"PreferredMaintenanceWindow\": {\n      \"type\": \"string\"\n    },\n    \"AutoMinorVersionUpgrade\": {\n      \"type\": \"boolean\"\n    },\n    \"NewDBInstanceIdentifier\": {\n      \"type\": \"string\"\n    },\n    \"PromotionTier\": {\n      \"type\": \"integer\"\n    },\n    \"ApplyImmediately\": {\n      \"type\": \"boolean\"\n    }\n\
  \  },\n  \"required\": [\n    \"DBInstanceIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/management-modify-db-instance-request-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: ModifyDBInstanceRequest
---
