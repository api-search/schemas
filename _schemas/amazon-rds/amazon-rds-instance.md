---
description: Represents an Amazon RDS database instance with its associated configuration, state, endpoint, and metadata.
layout: schema
name: Amazon RDS DB Instance
properties_list:
- description: The user-supplied unique key that identifies the DB instance
  name: dBInstanceIdentifier
  type: string
- description: The name of the compute and memory capacity class of the DB instance (e.g., db.m5.large, db.r5.xlarge)
  name: dBInstanceClass
  type: string
- description: The database engine for this DB instance
  name: engine
  type: string
- description: The version number of the database engine
  name: engineVersion
  type: string
- description: The current state of the DB instance
  name: dBInstanceStatus
  type: string
- description: The master username for the DB instance
  name: masterUsername
  type: string
- description: The name of the initial database created when the DB instance was created
  name: dBName
  type: string
- description: ''
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
- description: ''
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
- description: The identifier of the CA certificate for this DB instance
  name: cACertificateIdentifier
  type: string
- description: The Amazon Resource Name (ARN) for the DB instance
  name: dBInstanceArn
  type: string
- description: Tags assigned to the DB instance
  name: tags
  type: array
- description: The port that the DB instance listens on
  name: port
  type: integer
- description: If the DB instance is a member of a DB cluster, the cluster identifier
  name: dBClusterIdentifier
  type: string
- description: The license model information for this DB instance
  name: licenseModel
  type: string
provider_name: Amazon RDS
provider_slug: amazon-rds
schema_file: json-schema/amazon-rds-instance-schema.json
slug: amazon-rds-instance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/amazon/rds/instance.json\",\n  \"title\": \"Amazon RDS DB Instance\",\n  \"description\": \"Represents an Amazon RDS database instance with its associated configuration, state, endpoint, and metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"dBInstanceIdentifier\", \"dBInstanceClass\", \"engine\", \"dBInstanceStatus\"],\n  \"properties\": {\n    \"dBInstanceIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The user-supplied unique key that identifies the DB instance\"\n    },\n    \"dBInstanceClass\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the compute and memory capacity class of the DB instance (e.g., db.m5.large, db.r5.xlarge)\"\n    },\n    \"engine\": {\n      \"type\": \"string\",\n      \"description\": \"The database engine for this DB instance\",\n      \"enum\": [\"mysql\", \"postgres\", \"mariadb\"\
  , \"oracle-ee\", \"oracle-se2\", \"sqlserver-ee\", \"sqlserver-se\", \"sqlserver-ex\", \"sqlserver-web\", \"aurora-mysql\", \"aurora-postgresql\"]\n    },\n    \"engineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version number of the database engine\"\n    },\n    \"dBInstanceStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the DB instance\",\n      \"enum\": [\"available\", \"backing-up\", \"creating\", \"deleting\", \"failed\", \"inaccessible-encryption-credentials\", \"incompatible-network\", \"incompatible-option-group\", \"incompatible-parameters\", \"incompatible-restore\", \"maintenance\", \"modifying\", \"moving-to-vpc\", \"rebooting\", \"renaming\", \"resetting-master-credentials\", \"restore-error\", \"starting\", \"stopped\", \"stopping\", \"storage-full\", \"storage-optimization\", \"upgrading\"]\n    },\n    \"masterUsername\": {\n      \"type\": \"string\",\n      \"description\": \"The master username for\
  \ the DB instance\"\n    },\n    \"dBName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the initial database created when the DB instance was created\"\n    },\n    \"endpoint\": {\n      \"$ref\": \"#/$defs/Endpoint\"\n    },\n    \"allocatedStorage\": {\n      \"type\": \"integer\",\n      \"description\": \"The allocated storage size in gibibytes (GiB)\",\n      \"minimum\": 20,\n      \"maximum\": 65536\n    },\n    \"instanceCreateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the DB instance was created\"\n    },\n    \"preferredBackupWindow\": {\n      \"type\": \"string\",\n      \"description\": \"The daily time range during which automated backups are created\"\n    },\n    \"backupRetentionPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of days for which automatic DB snapshots are retained\",\n      \"minimum\": 0,\n      \"maximum\": 35\n    },\n  \
  \  \"vpcSecurityGroups\": {\n      \"type\": \"array\",\n      \"description\": \"The VPC security groups associated with the DB instance\",\n      \"items\": {\n        \"$ref\": \"#/$defs/VpcSecurityGroupMembership\"\n      }\n    },\n    \"availabilityZone\": {\n      \"type\": \"string\",\n      \"description\": \"The Availability Zone where the DB instance is located\"\n    },\n    \"dBSubnetGroup\": {\n      \"$ref\": \"#/$defs/DBSubnetGroup\"\n    },\n    \"multiAZ\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the DB instance is a Multi-AZ deployment\"\n    },\n    \"autoMinorVersionUpgrade\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether minor version patches are applied automatically\"\n    },\n    \"storageType\": {\n      \"type\": \"string\",\n      \"description\": \"The storage type associated with the DB instance\",\n      \"enum\": [\"gp2\", \"gp3\", \"io1\", \"standard\"]\n    },\n    \"storageEncrypted\": {\n      \"type\": \"\
  boolean\",\n      \"description\": \"Whether the DB instance is encrypted\"\n    },\n    \"publiclyAccessible\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the DB instance is publicly accessible\"\n    },\n    \"cACertificateIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the CA certificate for this DB instance\"\n    },\n    \"dBInstanceArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the DB instance\",\n      \"pattern\": \"^arn:aws:rds:[a-z0-9-]+:[0-9]{12}:db:.+$\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags assigned to the DB instance\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      }\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port that the DB instance listens on\"\n    },\n    \"dBClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"If the DB instance\
  \ is a member of a DB cluster, the cluster identifier\"\n    },\n    \"licenseModel\": {\n      \"type\": \"string\",\n      \"description\": \"The license model information for this DB instance\"\n    }\n  },\n  \"$defs\": {\n    \"Endpoint\": {\n      \"type\": \"object\",\n      \"description\": \"The connection endpoint for the DB instance\",\n      \"properties\": {\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"The DNS address of the DB instance\"\n        },\n        \"port\": {\n          \"type\": \"integer\",\n          \"description\": \"The port that the DB instance listens on\"\n        },\n        \"hostedZoneId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the hosted zone associated with the DB instance\"\n        }\n      }\n    },\n    \"DBSubnetGroup\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the subnet group associated with the DB instance\",\n      \"properties\"\
  : {\n        \"dBSubnetGroupName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the DB subnet group\"\n        },\n        \"dBSubnetGroupDescription\": {\n          \"type\": \"string\",\n          \"description\": \"The description of the DB subnet group\"\n        },\n        \"vpcId\": {\n          \"type\": \"string\",\n          \"description\": \"The VPC ID of the DB subnet group\",\n          \"pattern\": \"^vpc-[a-f0-9]{8,17}$\"\n        },\n        \"subnetGroupStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the DB subnet group\"\n        },\n        \"subnets\": {\n          \"type\": \"array\",\n          \"description\": \"The subnets that belong to the DB subnet group\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"subnetIdentifier\": {\n                \"type\": \"string\",\n                \"description\": \"The identifier of the subnet\"\
  ,\n                \"pattern\": \"^subnet-[a-f0-9]{8,17}$\"\n              },\n              \"subnetAvailabilityZone\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"name\": {\n                    \"type\": \"string\",\n                    \"description\": \"The name of the Availability Zone\"\n                  }\n                }\n              },\n              \"subnetStatus\": {\n                \"type\": \"string\",\n                \"description\": \"The status of the subnet\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"VpcSecurityGroupMembership\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a VPC security group membership\",\n      \"properties\": {\n        \"vpcSecurityGroupId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the VPC security group\",\n          \"pattern\": \"^sg-[a-f0-9]{8,17}$\"\n        },\n        \"status\": {\n  \
  \        \"type\": \"string\",\n          \"description\": \"The membership status of the VPC security group\"\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a resource tag\",\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The key of the tag\",\n          \"maxLength\": 128\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The value of the tag\",\n          \"maxLength\": 256\n        }\n      },\n      \"required\": [\"key\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-rds/refs/heads/main/json-schema/amazon-rds-instance-schema.json
tags:
- AWS
- Cloud Databases
- Database Service
- DBaaS
- Managed Databases
- Relational Databases
title: Amazon RDS DB Instance
---
