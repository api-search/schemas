---
description: Describes an Amazon RDS DB instance
layout: schema
name: DBInstance
properties_list:
- description: The user-supplied unique key that identifies the DB instance
  name: dBInstanceIdentifier
  type: string
- description: The name of the compute and memory capacity class of the DB instance
  name: dBInstanceClass
  type: string
- description: The database engine for this DB instance
  name: engine
  type: string
- description: The version of the database engine
  name: engineVersion
  type: string
- description: The current state of the DB instance
  name: dBInstanceStatus
  type: string
- description: The master username for the DB instance
  name: masterUsername
  type: string
- description: The name of the initial database provided during creation
  name: dBName
  type: string
- description: The connection endpoint for the DB instance
  name: endpoint
  type: object
- description: The allocated storage size in gibibytes (GiB)
  name: allocatedStorage
  type: integer
- description: The date and time the DB instance was created
  name: instanceCreateTime
  type: string
- description: The daily time range during which automated backups are created
  name: preferredBackupWindow
  type: string
- description: The number of days for which automatic DB snapshots are retained
  name: backupRetentionPeriod
  type: integer
- description: The VPC security groups associated with the DB instance
  name: vpcSecurityGroups
  type: array
- description: The Availability Zone where the DB instance is located
  name: availabilityZone
  type: string
- description: Information about the subnet group associated with the DB instance
  name: dBSubnetGroup
  type: object
- description: Whether the DB instance is a Multi-AZ deployment
  name: multiAZ
  type: boolean
- description: Whether minor version patches are applied automatically
  name: autoMinorVersionUpgrade
  type: boolean
- description: The storage type associated with the DB instance
  name: storageType
  type: string
- description: Whether the DB instance is encrypted
  name: storageEncrypted
  type: boolean
- description: Whether the DB instance is publicly accessible
  name: publiclyAccessible
  type: boolean
- description: The Amazon Resource Name (ARN) for the DB instance
  name: dBInstanceArn
  type: string
- description: Tags assigned to the DB instance
  name: tags
  type: array
provider_name: Amazon RDS
provider_slug: amazon-rds
schema_file: json-schema/amazon-rds-openapi-db-instance-schema.json
slug: amazon-rds-openapi-db-instance
source_filename: amazon-rds-openapi-db-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-db-instance-schema.json\",\n  \"title\": \"DBInstance\",\n  \"description\": \"Describes an Amazon RDS DB instance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dBInstanceIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The user-supplied unique key that identifies the DB instance\"\n    },\n    \"dBInstanceClass\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the compute and memory capacity class of the DB instance\"\n    },\n    \"engine\": {\n      \"type\": \"string\",\n      \"description\": \"The database engine for this DB instance\"\n    },\n    \"engineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the database engine\"\n    },\n    \"dBInstanceStatus\": {\n      \"type\": \"string\",\n   \
  \   \"description\": \"The current state of the DB instance\",\n      \"enum\": [\n        \"available\",\n        \"backing-up\",\n        \"configuring-enhanced-monitoring\",\n        \"configuring-iam-database-auth\",\n        \"configuring-log-exports\",\n        \"creating\",\n        \"delete-precheck\",\n        \"deleting\",\n        \"failed\",\n        \"inaccessible-encryption-credentials\",\n        \"incompatible-network\",\n        \"incompatible-option-group\",\n        \"incompatible-parameters\",\n        \"incompatible-restore\",\n        \"maintenance\",\n        \"modifying\",\n        \"moving-to-vpc\",\n        \"rebooting\",\n        \"renaming\",\n        \"resetting-master-credentials\",\n        \"restore-error\",\n        \"starting\",\n        \"stopped\",\n        \"stopping\",\n        \"storage-full\",\n        \"storage-optimization\",\n        \"upgrading\"\n      ]\n    },\n    \"masterUsername\": {\n      \"type\": \"string\",\n      \"description\":\
  \ \"The master username for the DB instance\"\n    },\n    \"dBName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the initial database provided during creation\"\n    },\n    \"endpoint\": {\n      \"type\": \"object\",\n      \"description\": \"The connection endpoint for the DB instance\",\n      \"properties\": {\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"The DNS address of the DB instance\"\n        },\n        \"port\": {\n          \"type\": \"integer\",\n          \"description\": \"The port that the DB instance listens on\"\n        },\n        \"hostedZoneId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the hosted zone for the DB instance\"\n        }\n      }\n    },\n    \"allocatedStorage\": {\n      \"type\": \"integer\",\n      \"description\": \"The allocated storage size in gibibytes (GiB)\"\n    },\n    \"instanceCreateTime\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"The date and time the DB instance was created\"\n    },\n    \"preferredBackupWindow\": {\n      \"type\": \"string\",\n      \"description\": \"The daily time range during which automated backups are created\"\n    },\n    \"backupRetentionPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of days for which automatic DB snapshots are retained\"\n    },\n    \"vpcSecurityGroups\": {\n      \"type\": \"array\",\n      \"description\": \"The VPC security groups associated with the DB instance\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"vpcSecurityGroupId\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the VPC security group\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"description\": \"The membership status of the VPC security group\"\n          }\n        }\n      }\n    },\n    \"availabilityZone\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The Availability Zone where the DB instance is located\"\n    },\n    \"dBSubnetGroup\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the subnet group associated with the DB instance\",\n      \"properties\": {\n        \"dBSubnetGroupName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the DB subnet group\"\n        },\n        \"dBSubnetGroupDescription\": {\n          \"type\": \"string\",\n          \"description\": \"The description of the DB subnet group\"\n        },\n        \"vpcId\": {\n          \"type\": \"string\",\n          \"description\": \"The VPC ID of the DB subnet group\"\n        }\n      }\n    },\n    \"multiAZ\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the DB instance is a Multi-AZ deployment\"\n    },\n    \"autoMinorVersionUpgrade\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether minor version patches\
  \ are applied automatically\"\n    },\n    \"storageType\": {\n      \"type\": \"string\",\n      \"description\": \"The storage type associated with the DB instance\"\n    },\n    \"storageEncrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the DB instance is encrypted\"\n    },\n    \"publiclyAccessible\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the DB instance is publicly accessible\"\n    },\n    \"dBInstanceArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the DB instance\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags assigned to the DB instance\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-openapi-db-instance-schema.json
tags:
- AWS
- Cloud Databases
- Database Service
- DBaaS
- Managed Databases
- Relational Databases
title: DBInstance
---
