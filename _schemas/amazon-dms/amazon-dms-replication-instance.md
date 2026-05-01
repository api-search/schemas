---
description: Provides information that defines a replication instance.
layout: schema
name: ReplicationInstance
properties_list:
- description: ''
  name: ReplicationInstanceIdentifier
  type: object
- description: ''
  name: ReplicationInstanceClass
  type: object
- description: ''
  name: ReplicationInstanceStatus
  type: object
- description: ''
  name: AllocatedStorage
  type: object
- description: ''
  name: InstanceCreateTime
  type: object
- description: ''
  name: VpcSecurityGroups
  type: object
- description: ''
  name: AvailabilityZone
  type: object
- description: ''
  name: ReplicationSubnetGroup
  type: object
- description: ''
  name: PreferredMaintenanceWindow
  type: object
- description: ''
  name: PendingModifiedValues
  type: object
- description: ''
  name: MultiAZ
  type: object
- description: ''
  name: EngineVersion
  type: object
- description: ''
  name: AutoMinorVersionUpgrade
  type: object
- description: ''
  name: KmsKeyId
  type: object
- description: ''
  name: ReplicationInstanceArn
  type: object
- description: ''
  name: ReplicationInstancePublicIpAddress
  type: object
- description: ''
  name: ReplicationInstancePrivateIpAddress
  type: object
- description: ''
  name: ReplicationInstancePublicIpAddresses
  type: object
- description: ''
  name: ReplicationInstancePrivateIpAddresses
  type: object
- description: ''
  name: ReplicationInstanceIpv6Addresses
  type: object
- description: ''
  name: PubliclyAccessible
  type: object
- description: ''
  name: SecondaryAvailabilityZone
  type: object
- description: ''
  name: FreeUntil
  type: object
- description: ''
  name: DnsNameServers
  type: object
- description: ''
  name: NetworkType
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-replication-instance-schema.json
slug: amazon-dms-replication-instance
source_filename: amazon-dms-replication-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-replication-instance-schema.json\",\n  \"title\": \"ReplicationInstance\",\n  \"description\": \"Provides information that defines a replication instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReplicationInstanceIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The replication instance identifier is a required parameter. This parameter is stored as a lowercase string.</p> <p>Constraints:</p> <ul> <li> <p>Must contain 1-63 alphanumeric characters or hyphens.</p> </li> <li> <p>First character must be a letter.</p> </li> <li> <p>Cannot end with a hyphen or contain two consecutive hyphens.</p> </li> </ul> <p>Example: <code>myrepinstance</code> </p>\"\n        }\n      ]\n    },\n\
  \    \"ReplicationInstanceClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The compute and memory capacity of the replication instance as defined for the specified replication instance class. It is a required parameter, although a default value is pre-selected in the DMS console.</p> <p>For more information on the settings and capacities for the available replication instance classes, see <a href=\\\"https://docs.aws.amazon.com/dms/latest/userguide/CHAP_ReplicationInstance.html#CHAP_ReplicationInstance.InDepth\\\"> Selecting the right DMS replication instance for your migration</a>. </p>\"\n        }\n      ]\n    },\n    \"ReplicationInstanceStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The status of the replication instance. The possible return values include:</p> <ul> <li> <p> <code>\\\
  \"available\\\"</code> </p> </li> <li> <p> <code>\\\"creating\\\"</code> </p> </li> <li> <p> <code>\\\"deleted\\\"</code> </p> </li> <li> <p> <code>\\\"deleting\\\"</code> </p> </li> <li> <p> <code>\\\"failed\\\"</code> </p> </li> <li> <p> <code>\\\"modifying\\\"</code> </p> </li> <li> <p> <code>\\\"upgrading\\\"</code> </p> </li> <li> <p> <code>\\\"rebooting\\\"</code> </p> </li> <li> <p> <code>\\\"resetting-master-credentials\\\"</code> </p> </li> <li> <p> <code>\\\"storage-full\\\"</code> </p> </li> <li> <p> <code>\\\"incompatible-credentials\\\"</code> </p> </li> <li> <p> <code>\\\"incompatible-network\\\"</code> </p> </li> <li> <p> <code>\\\"maintenance\\\"</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"AllocatedStorage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The amount of storage (in gigabytes) that is allocated for the replication instance.\"\n        }\n      ]\n\
  \    },\n    \"InstanceCreateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The time the replication instance was created.\"\n        }\n      ]\n    },\n    \"VpcSecurityGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcSecurityGroupMembershipList\"\n        },\n        {\n          \"description\": \"The VPC security group for the instance.\"\n        }\n      ]\n    },\n    \"AvailabilityZone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Availability Zone for the instance.\"\n        }\n      ]\n    },\n    \"ReplicationSubnetGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReplicationSubnetGroup\"\n        },\n        {\n          \"description\": \"The subnet group for the replication instance.\"\n        }\n\
  \      ]\n    },\n    \"PreferredMaintenanceWindow\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The maintenance window times for the replication instance. Any pending upgrades to the replication instance are performed during this time.\"\n        }\n      ]\n    },\n    \"PendingModifiedValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReplicationPendingModifiedValues\"\n        },\n        {\n          \"description\": \"The pending modification values.\"\n        }\n      ]\n    },\n    \"MultiAZ\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \" Specifies whether the replication instance is a Multi-AZ deployment. You can't set the <code>AvailabilityZone</code> parameter if the Multi-AZ parameter is set to <code>true</code>. \"\n        }\n      ]\n    },\n   \
  \ \"EngineVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The engine version number of the replication instance.</p> <p>If an engine version number is not specified when a replication instance is created, the default is the latest engine version available.</p> <p>When modifying a major engine version of an instance, also set <code>AllowMajorVersionUpgrade</code> to <code>true</code>.</p>\"\n        }\n      ]\n    },\n    \"AutoMinorVersionUpgrade\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Boolean value indicating if minor version upgrades will be automatically applied to the instance.\"\n        }\n      ]\n    },\n    \"KmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>An KMS key\
  \ identifier that is used to encrypt the data on the replication instance.</p> <p>If you don't specify a value for the <code>KmsKeyId</code> parameter, then DMS uses your default encryption key.</p> <p>KMS creates the default encryption key for your Amazon Web Services account. Your Amazon Web Services account has a different default encryption key for each Amazon Web Services Region.</p>\"\n        }\n      ]\n    },\n    \"ReplicationInstanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the replication instance.\"\n        }\n      ]\n    },\n    \"ReplicationInstancePublicIpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"The public IP address of the replication instance.\"\n        }\n      ]\n    },\n    \"ReplicationInstancePrivateIpAddress\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"The private IP address of the replication instance.\"\n        }\n      ]\n    },\n    \"ReplicationInstancePublicIpAddresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReplicationInstancePublicIpAddressList\"\n        },\n        {\n          \"description\": \"One or more public IP addresses for the replication instance.\"\n        }\n      ]\n    },\n    \"ReplicationInstancePrivateIpAddresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReplicationInstancePrivateIpAddressList\"\n        },\n        {\n          \"description\": \"One or more private IP addresses for the replication instance.\"\n        }\n      ]\n    },\n    \"ReplicationInstanceIpv6Addresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReplicationInstanceIpv6AddressList\"\
  \n        },\n        {\n          \"description\": \"One or more IPv6 addresses for the replication instance.\"\n        }\n      ]\n    },\n    \"PubliclyAccessible\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \" Specifies the accessibility options for the replication instance. A value of <code>true</code> represents an instance with a public IP address. A value of <code>false</code> represents an instance with a private IP address. The default value is <code>true</code>. \"\n        }\n      ]\n    },\n    \"SecondaryAvailabilityZone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Availability Zone of the standby replication instance in a Multi-AZ deployment.\"\n        }\n      ]\n    },\n    \"FreeUntil\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\
  \n        },\n        {\n          \"description\": \" The expiration date of the free replication instance that is part of the Free DMS program. \"\n        }\n      ]\n    },\n    \"DnsNameServers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The DNS name servers supported for the replication instance to access your on-premise source or target database.\"\n        }\n      ]\n    },\n    \"NetworkType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type of IP address protocol used by a replication instance, such as IPv4 only or Dual-stack that supports both IPv4 and IPv6 addressing. IPv6 only is not yet supported.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-replication-instance-schema.json
tags:
- Data Replication
- Database
- Database Migration
- Migration
title: ReplicationInstance
---
