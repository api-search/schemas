---
description: Describes an Amazon RDS DB snapshot
layout: schema
name: DBSnapshot
properties_list:
- description: The identifier for the DB snapshot
  name: dBSnapshotIdentifier
  type: string
- description: The DB instance identifier of the source DB instance
  name: dBInstanceIdentifier
  type: string
- description: The time when the snapshot was taken
  name: snapshotCreateTime
  type: string
- description: The database engine for the snapshot
  name: engine
  type: string
- description: The version of the database engine
  name: engineVersion
  type: string
- description: The status of the DB snapshot
  name: status
  type: string
- description: The allocated storage size in GiB
  name: allocatedStorage
  type: integer
- description: The port that the database engine was listening on at snapshot time
  name: port
  type: integer
- description: The Availability Zone where the snapshot was created
  name: availabilityZone
  type: string
- description: The VPC ID associated with the DB snapshot
  name: vpcId
  type: string
- description: The time when the source DB instance was created
  name: instanceCreateTime
  type: string
- description: The master username for the DB snapshot
  name: masterUsername
  type: string
- description: The type of the DB snapshot
  name: snapshotType
  type: string
- description: Whether the DB snapshot is encrypted
  name: encrypted
  type: boolean
- description: The storage type associated with the DB snapshot
  name: storageType
  type: string
- description: The Amazon Resource Name (ARN) for the DB snapshot
  name: dBSnapshotArn
  type: string
- description: Tags assigned to the DB snapshot
  name: tags
  type: array
provider_name: Amazon RDS
provider_slug: amazon-rds
schema_file: json-schema/amazon-rds-openapi-db-snapshot-schema.json
slug: amazon-rds-openapi-db-snapshot
source_filename: amazon-rds-openapi-db-snapshot-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-db-snapshot-schema.json\",\n  \"title\": \"DBSnapshot\",\n  \"description\": \"Describes an Amazon RDS DB snapshot\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dBSnapshotIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier for the DB snapshot\"\n    },\n    \"dBInstanceIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The DB instance identifier of the source DB instance\"\n    },\n    \"snapshotCreateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the snapshot was taken\"\n    },\n    \"engine\": {\n      \"type\": \"string\",\n      \"description\": \"The database engine for the snapshot\"\n    },\n    \"engineVersion\": {\n      \"type\": \"string\",\n      \"\
  description\": \"The version of the database engine\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the DB snapshot\",\n      \"enum\": [\n        \"available\",\n        \"creating\",\n        \"deleting\",\n        \"copying\"\n      ]\n    },\n    \"allocatedStorage\": {\n      \"type\": \"integer\",\n      \"description\": \"The allocated storage size in GiB\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port that the database engine was listening on at snapshot time\"\n    },\n    \"availabilityZone\": {\n      \"type\": \"string\",\n      \"description\": \"The Availability Zone where the snapshot was created\"\n    },\n    \"vpcId\": {\n      \"type\": \"string\",\n      \"description\": \"The VPC ID associated with the DB snapshot\"\n    },\n    \"instanceCreateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the source DB instance\
  \ was created\"\n    },\n    \"masterUsername\": {\n      \"type\": \"string\",\n      \"description\": \"The master username for the DB snapshot\"\n    },\n    \"snapshotType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the DB snapshot\",\n      \"enum\": [\n        \"automated\",\n        \"manual\",\n        \"shared\",\n        \"public\",\n        \"awsbackup\"\n      ]\n    },\n    \"encrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the DB snapshot is encrypted\"\n    },\n    \"storageType\": {\n      \"type\": \"string\",\n      \"description\": \"The storage type associated with the DB snapshot\"\n    },\n    \"dBSnapshotArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the DB snapshot\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags assigned to the DB snapshot\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n     \
  \ }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-db-snapshot-schema.json
tags:
- Cloud Databases
- Database Service
- DBaaS
- Managed Databases
- Relational Databases
title: DBSnapshot
---
