---
description: Schema for an Amazon Redshift provisioned cluster resource, representing a fully managed petabyte-scale data warehouse in the AWS cloud. Includes cluster configuration, networking, security, and operational metadata as described in the Amazon Redshift Management Guide.
layout: schema
name: Amazon Redshift Cluster
properties_list:
- description: The unique identifier of the cluster. Must be lowercase, begin with a letter, contain only alphanumeric characters and hyphens, and be between 1 and 63 characters.
  name: ClusterIdentifier
  type: string
- description: The current state of the cluster
  name: ClusterStatus
  type: string
- description: The availability status of the cluster for queries
  name: ClusterAvailabilityStatus
  type: string
- description: The node type for the nodes in the cluster
  name: NodeType
  type: string
- description: The number of compute nodes in the cluster. For single-node clusters this is 1.
  name: NumberOfNodes
  type: integer
- description: The type of the cluster based on number of nodes
  name: ClusterType
  type: string
- description: The name of the initial database created when the cluster was provisioned. Default is 'dev'.
  name: DBName
  type: string
- description: The admin user name for the cluster. Must be lowercase, begin with a letter, contain only alphanumeric characters, and be between 1 and 128 characters.
  name: MasterUsername
  type: string
- description: ''
  name: Endpoint
  type: object
- description: The date and time that the cluster was created
  name: ClusterCreateTime
  type: string
- description: The number of days that automatic cluster snapshots are retained. Default is 1.
  name: AutomatedSnapshotRetentionPeriod
  type: integer
- description: The default number of days to retain a manual snapshot. -1 means indefinitely.
  name: ManualSnapshotRetentionPeriod
  type: integer
- description: List of cluster security groups associated with the cluster
  name: ClusterSecurityGroups
  type: array
- description: List of VPC security groups associated with the cluster
  name: VpcSecurityGroups
  type: array
- description: List of cluster parameter groups associated with this cluster
  name: ClusterParameterGroups
  type: array
- description: The name of the subnet group associated with the cluster
  name: ClusterSubnetGroupName
  type: string
- description: The identifier of the VPC the cluster is in
  name: VpcId
  type: string
- description: The name of the Availability Zone in which the cluster is located
  name: AvailabilityZone
  type: string
- description: The weekly time range for system maintenance in UTC, formatted as ddd:hh24:mi-ddd:hh24:mi
  name: PreferredMaintenanceWindow
  type: string
- description: The version ID of the Amazon Redshift engine running on the cluster
  name: ClusterVersion
  type: string
- description: Whether major version upgrades are applied automatically during the maintenance window
  name: AllowVersionUpgrade
  type: boolean
- description: Whether the cluster can be accessed from a public network
  name: PubliclyAccessible
  type: boolean
- description: Whether data in the cluster is encrypted at rest
  name: Encrypted
  type: boolean
- description: The AWS KMS key ID used for encryption of data at rest
  name: KmsKeyId
  type: string
- description: Whether enhanced VPC routing is enabled, forcing all COPY and UNLOAD traffic through the VPC
  name: EnhancedVpcRouting
  type: boolean
- description: List of IAM roles associated with the cluster for authorization
  name: IamRoles
  type: array
- description: The name of the maintenance track for the cluster
  name: MaintenanceTrackName
  type: string
- description: The number of nodes that you can resize the cluster to using elastic resize
  name: ElasticResizeNumberOfNodeOptions
  type: string
- description: ''
  name: AquaConfiguration
  type: object
- description: The total storage capacity of the cluster in megabytes
  name: TotalStorageCapacityInMegaBytes
  type: integer
- description: The namespace ARN of the cluster
  name: ClusterNamespaceArn
  type: string
- description: Tags associated with the cluster
  name: Tags
  type: array
provider_name: Amazon Redshift
provider_slug: amazon-redshift
schema_file: json-schema/amazon-redshift-cluster-schema.json
slug: amazon-redshift-cluster
source_filename: amazon-redshift-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://aws.amazon.com/schemas/redshift/cluster.json\",\n  \"title\": \"Amazon Redshift Cluster\",\n  \"description\": \"Schema for an Amazon Redshift provisioned cluster resource, representing a fully managed petabyte-scale data warehouse in the AWS cloud. Includes cluster configuration, networking, security, and operational metadata as described in the Amazon Redshift Management Guide.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"ClusterIdentifier\",\n    \"NodeType\",\n    \"MasterUsername\",\n    \"DBName\"\n  ],\n  \"properties\": {\n    \"ClusterIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the cluster. Must be lowercase, begin with a letter, contain only alphanumeric characters and hyphens, and be between 1 and 63 characters.\",\n      \"pattern\": \"^[a-z][a-z0-9-]*$\",\n      \"minLength\": 1,\n      \"maxLength\": 63,\n     \
  \ \"examples\": [\"my-redshift-cluster\"]\n    },\n    \"ClusterStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the cluster\",\n      \"enum\": [\n        \"available\",\n        \"creating\",\n        \"deleting\",\n        \"final-snapshot\",\n        \"hardware-failure\",\n        \"incompatible-hsm\",\n        \"incompatible-network\",\n        \"incompatible-parameters\",\n        \"incompatible-restore\",\n        \"modifying\",\n        \"paused\",\n        \"rebooting\",\n        \"renaming\",\n        \"resizing\",\n        \"rotating-keys\",\n        \"storage-full\",\n        \"updating-hsm\"\n      ]\n    },\n    \"ClusterAvailabilityStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The availability status of the cluster for queries\",\n      \"enum\": [\n        \"Available\",\n        \"Unavailable\",\n        \"Maintenance\",\n        \"Modifying\"\n      ]\n    },\n    \"NodeType\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"The node type for the nodes in the cluster\",\n      \"enum\": [\n        \"dc2.large\",\n        \"dc2.8xlarge\",\n        \"ra3.xlplus\",\n        \"ra3.4xlarge\",\n        \"ra3.16xlarge\"\n      ]\n    },\n    \"NumberOfNodes\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of compute nodes in the cluster. For single-node clusters this is 1.\",\n      \"minimum\": 1,\n      \"maximum\": 128,\n      \"default\": 1\n    },\n    \"ClusterType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the cluster based on number of nodes\",\n      \"enum\": [\n        \"single-node\",\n        \"multi-node\"\n      ]\n    },\n    \"DBName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the initial database created when the cluster was provisioned. Default is 'dev'.\",\n      \"default\": \"dev\",\n      \"examples\": [\"dev\", \"mydb\"]\n    },\n    \"MasterUsername\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"The admin user name for the cluster. Must be lowercase, begin with a letter, contain only alphanumeric characters, and be between 1 and 128 characters.\",\n      \"minLength\": 1,\n      \"maxLength\": 128\n    },\n    \"Endpoint\": {\n      \"$ref\": \"#/$defs/Endpoint\"\n    },\n    \"ClusterCreateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time that the cluster was created\"\n    },\n    \"AutomatedSnapshotRetentionPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of days that automatic cluster snapshots are retained. Default is 1.\",\n      \"minimum\": 0,\n      \"maximum\": 35,\n      \"default\": 1\n    },\n    \"ManualSnapshotRetentionPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"The default number of days to retain a manual snapshot. -1 means indefinitely.\",\n      \"minimum\": -1,\n      \"maximum\": 3653,\n      \"default\": -1\n \
  \   },\n    \"ClusterSecurityGroups\": {\n      \"type\": \"array\",\n      \"description\": \"List of cluster security groups associated with the cluster\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ClusterSecurityGroupMembership\"\n      }\n    },\n    \"VpcSecurityGroups\": {\n      \"type\": \"array\",\n      \"description\": \"List of VPC security groups associated with the cluster\",\n      \"items\": {\n        \"$ref\": \"#/$defs/VpcSecurityGroupMembership\"\n      }\n    },\n    \"ClusterParameterGroups\": {\n      \"type\": \"array\",\n      \"description\": \"List of cluster parameter groups associated with this cluster\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ClusterParameterGroupStatus\"\n      }\n    },\n    \"ClusterSubnetGroupName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the subnet group associated with the cluster\"\n    },\n    \"VpcId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the VPC\
  \ the cluster is in\",\n      \"pattern\": \"^vpc-[a-z0-9]+$\",\n      \"examples\": [\"vpc-0abc123def456\"]\n    },\n    \"AvailabilityZone\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Availability Zone in which the cluster is located\",\n      \"examples\": [\"us-east-1a\"]\n    },\n    \"PreferredMaintenanceWindow\": {\n      \"type\": \"string\",\n      \"description\": \"The weekly time range for system maintenance in UTC, formatted as ddd:hh24:mi-ddd:hh24:mi\",\n      \"examples\": [\"sun:05:00-sun:05:30\"]\n    },\n    \"ClusterVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version ID of the Amazon Redshift engine running on the cluster\",\n      \"examples\": [\"1.0\"]\n    },\n    \"AllowVersionUpgrade\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether major version upgrades are applied automatically during the maintenance window\",\n      \"default\": true\n    },\n    \"PubliclyAccessible\": {\n      \"\
  type\": \"boolean\",\n      \"description\": \"Whether the cluster can be accessed from a public network\",\n      \"default\": false\n    },\n    \"Encrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether data in the cluster is encrypted at rest\",\n      \"default\": false\n    },\n    \"KmsKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS KMS key ID used for encryption of data at rest\",\n      \"examples\": [\"arn:aws:kms:us-east-1:123456789012:key/abcd1234-ef56-gh78-ij90-klmn1234opqr\"]\n    },\n    \"EnhancedVpcRouting\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether enhanced VPC routing is enabled, forcing all COPY and UNLOAD traffic through the VPC\",\n      \"default\": false\n    },\n    \"IamRoles\": {\n      \"type\": \"array\",\n      \"description\": \"List of IAM roles associated with the cluster for authorization\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ClusterIamRole\"\n      }\n    },\n    \"\
  MaintenanceTrackName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the maintenance track for the cluster\",\n      \"enum\": [\n        \"current\",\n        \"trailing\"\n      ],\n      \"default\": \"current\"\n    },\n    \"ElasticResizeNumberOfNodeOptions\": {\n      \"type\": \"string\",\n      \"description\": \"The number of nodes that you can resize the cluster to using elastic resize\"\n    },\n    \"AquaConfiguration\": {\n      \"$ref\": \"#/$defs/AquaConfiguration\"\n    },\n    \"TotalStorageCapacityInMegaBytes\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The total storage capacity of the cluster in megabytes\"\n    },\n    \"ClusterNamespaceArn\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace ARN of the cluster\",\n      \"examples\": [\"arn:aws:redshift:us-east-1:123456789012:namespace:abcd1234-ef56-gh78-ij90\"]\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"\
  description\": \"Tags associated with the cluster\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Endpoint\": {\n      \"type\": \"object\",\n      \"description\": \"Connection endpoint for the cluster\",\n      \"properties\": {\n        \"Address\": {\n          \"type\": \"string\",\n          \"description\": \"The DNS address of the cluster endpoint\",\n          \"examples\": [\"my-redshift-cluster.abc123xyz.us-east-1.redshift.amazonaws.com\"]\n        },\n        \"Port\": {\n          \"type\": \"integer\",\n          \"description\": \"The port that the database engine is listening on\",\n          \"default\": 5439,\n          \"examples\": [5439]\n        },\n        \"VpcEndpoints\": {\n          \"type\": \"array\",\n          \"description\": \"List of VPC endpoints for the cluster\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"VpcEndpointId\": {\n      \
  \          \"type\": \"string\",\n                \"description\": \"The VPC endpoint identifier\"\n              },\n              \"VpcId\": {\n                \"type\": \"string\",\n                \"description\": \"The VPC identifier\"\n              },\n              \"NetworkInterfaces\": {\n                \"type\": \"array\",\n                \"description\": \"Network interfaces of the endpoint\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"NetworkInterfaceId\": {\n                      \"type\": \"string\",\n                      \"description\": \"The network interface identifier\"\n                    },\n                    \"SubnetId\": {\n                      \"type\": \"string\",\n                      \"description\": \"The subnet identifier\"\n                    },\n                    \"PrivateIpAddress\": {\n                      \"type\": \"string\",\n                      \"\
  format\": \"ipv4\",\n                      \"description\": \"The private IP address of the interface\"\n                    },\n                    \"AvailabilityZone\": {\n                      \"type\": \"string\",\n                      \"description\": \"The Availability Zone\"\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"ClusterSecurityGroupMembership\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a cluster security group membership\",\n      \"properties\": {\n        \"ClusterSecurityGroupName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the cluster security group\"\n        },\n        \"Status\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the cluster security group\",\n          \"enum\": [\"active\", \"adding\", \"removing\"]\n        }\n      }\n    },\n    \"VpcSecurityGroupMembership\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Describes a VPC security group membership\",\n      \"properties\": {\n        \"VpcSecurityGroupId\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the VPC security group\"\n        },\n        \"Status\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the VPC security group\",\n          \"enum\": [\"active\", \"adding\", \"removing\"]\n        }\n      }\n    },\n    \"ClusterParameterGroupStatus\": {\n      \"type\": \"object\",\n      \"description\": \"Describes the status of a cluster parameter group\",\n      \"properties\": {\n        \"ParameterGroupName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the cluster parameter group\"\n        },\n        \"ParameterApplyStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The status of parameter updates\",\n          \"enum\": [\"in-sync\", \"pending-reboot\"\
  ]\n        },\n        \"ClusterParameterStatusList\": {\n          \"type\": \"array\",\n          \"description\": \"List of individual parameter statuses\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"ParameterName\": {\n                \"type\": \"string\",\n                \"description\": \"The name of the parameter\"\n              },\n              \"ParameterApplyType\": {\n                \"type\": \"string\",\n                \"description\": \"The apply type of the parameter\",\n                \"enum\": [\"static\", \"dynamic\"]\n              },\n              \"ParameterApplyStatus\": {\n                \"type\": \"string\",\n                \"description\": \"The status of the parameter\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"ClusterIamRole\": {\n      \"type\": \"object\",\n      \"description\": \"An IAM role associated with the cluster\",\n      \"properties\": {\n\
  \        \"IamRoleArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the IAM role\",\n          \"pattern\": \"^arn:aws:iam::\\\\d{12}:role/.+$\",\n          \"examples\": [\"arn:aws:iam::123456789012:role/RedshiftCopyRole\"]\n        },\n        \"ApplyStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the IAM role association\",\n          \"enum\": [\"in-sync\", \"adding\", \"removing\"]\n        }\n      }\n    },\n    \"AquaConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"AQUA (Advanced Query Accelerator) configuration for the cluster\",\n      \"properties\": {\n        \"AquaStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The value represents how the cluster is configured for using AQUA\",\n          \"enum\": [\"enabled\", \"disabled\", \"applying\"]\n        },\n        \"AquaConfigurationStatus\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The user-configured AQUA setting\",\n          \"enum\": [\"enabled\", \"disabled\", \"auto\"]\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"A tag consisting of a key-value pair\",\n      \"required\": [\"Key\"],\n      \"properties\": {\n        \"Key\": {\n          \"type\": \"string\",\n          \"description\": \"The key of the tag. Maximum 128 Unicode characters.\",\n          \"maxLength\": 128\n        },\n        \"Value\": {\n          \"type\": \"string\",\n          \"description\": \"The value of the tag. Maximum 256 Unicode characters.\",\n          \"maxLength\": 256\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-redshift/refs/heads/main/json-schema/amazon-redshift-cluster-schema.json
tags:
- Analytics
- Big Data
- Cloud
- Data Lake
- Data Warehouse
- ETL
- Machine Learning
- Serverless
- SQL
title: Amazon Redshift Cluster
---
