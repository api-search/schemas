---
description: Schema representing a CockroachDB Cloud cluster, which is an instance of CockroachDB running in one or more cloud regions on Serverless or Dedicated infrastructure.
layout: schema
name: CockroachDB Cluster
properties_list:
- description: Unique identifier of the cluster assigned by CockroachDB Cloud.
  name: id
  type: string
- description: Human-readable name of the cluster.
  name: name
  type: string
- description: Cloud infrastructure provider hosting the cluster.
  name: cloud_provider
  type: string
- description: Version string of CockroachDB running on the cluster (e.g. v23.1.0).
  name: cockroach_version
  type: string
- description: Service tier of the cluster, either Serverless or Dedicated.
  name: plan
  type: string
- description: Overall lifecycle state of the cluster.
  name: state
  type: string
- description: Current operational status reflecting any in-progress or failed operations.
  name: operation_status
  type: string
- description: Cloud provider regions where the cluster is deployed. Multi-region clusters have multiple entries.
  name: regions
  type: array
- description: Configuration settings for the cluster, containing either serverless or dedicated configuration.
  name: config
  type: object
- description: Identifier of the user who created the cluster.
  name: creator_id
  type: string
- description: RFC3339 timestamp when the cluster was created.
  name: created_at
  type: string
- description: RFC3339 timestamp of the most recent modification to the cluster.
  name: updated_at
  type: string
- description: RFC3339 timestamp when the cluster was deleted. Only present for deleted clusters.
  name: deleted_at
  type: string
- description: DNS hostname used for SQL connections to the cluster.
  name: sql_dns
  type: string
- description: Status of any in-progress version upgrade operation.
  name: upgrade_status
  type: string
- description: Cloud provider account ID for the cluster, used for trust relationship configuration.
  name: account_id
  type: string
- description: Folder ID of the folder containing this cluster, if any.
  name: parent_id
  type: string
- description: User-defined key-value labels attached to the cluster for organization and filtering.
  name: labels
  type: object
- description: Whether delete protection is enabled, preventing accidental cluster deletion.
  name: delete_protection
  type: string
- description: Policy governing outbound network traffic from the cluster.
  name: egress_traffic_policy
  type: string
- description: Network accessibility configuration controlling whether the cluster is publicly accessible.
  name: network_visibility
  type: string
- description: Client ID of the Azure cluster identity, present for Azure deployments that support CMEK.
  name: azure_cluster_identity_client_id
  type: string
- description: IPv4 CIDR range reserved for the cluster. Only set on GCP Advanced tier clusters.
  name: cidr_range
  type: string
- description: Customer cloud account details for BYOC (Bring Your Own Cloud) deployments.
  name: customer_cloud_account
  type: object
provider_name: CockroachDB
provider_slug: cockroachdb
schema_file: json-schema/cockroachdb-cluster-schema.json
slug: cockroachdb-cluster
source_filename: cockroachdb-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cockroachlabs.com/schemas/cockroachdb/cluster.json\",\n  \"title\": \"CockroachDB Cluster\",\n  \"description\": \"Schema representing a CockroachDB Cloud cluster, which is an instance of CockroachDB running in one or more cloud regions on Serverless or Dedicated infrastructure.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"cloud_provider\", \"state\", \"operation_status\", \"plan\", \"regions\", \"cockroach_version\", \"creator_id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the cluster assigned by CockroachDB Cloud.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the cluster.\",\n      \"maxLength\": 40\n    },\n    \"cloud_provider\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud infrastructure provider hosting the cluster.\"\
  ,\n      \"enum\": [\"GCP\", \"AWS\", \"AZURE\"]\n    },\n    \"cockroach_version\": {\n      \"type\": \"string\",\n      \"description\": \"Version string of CockroachDB running on the cluster (e.g. v23.1.0).\",\n      \"pattern\": \"^v[0-9]+\\\\.[0-9]+\\\\.[0-9]+\"\n    },\n    \"plan\": {\n      \"type\": \"string\",\n      \"description\": \"Service tier of the cluster, either Serverless or Dedicated.\",\n      \"enum\": [\"DEDICATED\", \"SERVERLESS\"]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Overall lifecycle state of the cluster.\",\n      \"enum\": [\"CREATING\", \"CREATED\", \"CREATION_FAILED\", \"DELETED\", \"LOCKED\"]\n    },\n    \"operation_status\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational status reflecting any in-progress or failed operations.\",\n      \"enum\": [\"CLUSTER_STATUS_UNSPECIFIED\", \"CRDB_MAJOR_UPGRADE_RUNNING\", \"CRDB_MAJOR_ROLLBACK_RUNNING\", \"CRDB_PATCH_RUNNING\", \"CRDB_SCALE_RUNNING\"\
  , \"TENANT_RESTORE_RUNNING\", \"CRDB_MAJOR_UPGRADE_PENDING\", \"CRDB_MAJOR_ROLLBACK_PENDING\", \"CRDB_PATCH_PENDING\", \"CRDB_SCALE_PENDING\", \"NONE\"]\n    },\n    \"regions\": {\n      \"type\": \"array\",\n      \"description\": \"Cloud provider regions where the cluster is deployed. Multi-region clusters have multiple entries.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/Region\"\n      }\n    },\n    \"config\": {\n      \"$ref\": \"#/$defs/ClusterConfig\",\n      \"description\": \"Configuration settings for the cluster, containing either serverless or dedicated configuration.\"\n    },\n    \"creator_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the user who created the cluster.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"RFC3339 timestamp when the cluster was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"\
  format\": \"date-time\",\n      \"description\": \"RFC3339 timestamp of the most recent modification to the cluster.\"\n    },\n    \"deleted_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"RFC3339 timestamp when the cluster was deleted. Only present for deleted clusters.\"\n    },\n    \"sql_dns\": {\n      \"type\": \"string\",\n      \"description\": \"DNS hostname used for SQL connections to the cluster.\"\n    },\n    \"upgrade_status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of any in-progress version upgrade operation.\",\n      \"enum\": [\"UPGRADE_AVAILABLE\", \"UPGRADING\", \"UPGRADE_QUEUED\", \"ROLLBACK_RUNNING\", \"FINALIZATION_PENDING\", \"FINALIZATION_FAILED\", \"MAJOR_UPGRADE_RUNNING\"]\n    },\n    \"account_id\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud provider account ID for the cluster, used for trust relationship configuration.\"\n    },\n    \"parent_id\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Folder ID of the folder containing this cluster, if any.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\": \"User-defined key-value labels attached to the cluster for organization and filtering.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"delete_protection\": {\n      \"type\": \"string\",\n      \"description\": \"Whether delete protection is enabled, preventing accidental cluster deletion.\",\n      \"enum\": [\"DELETE_PROTECTION_ENABLED\", \"DELETE_PROTECTION_DISABLED\"]\n    },\n    \"egress_traffic_policy\": {\n      \"type\": \"string\",\n      \"description\": \"Policy governing outbound network traffic from the cluster.\",\n      \"enum\": [\"EGRESS_TRAFFIC_POLICY_UNSPECIFIED\", \"DEFAULT_ALLOW\", \"DEFAULT_DENY\"]\n    },\n    \"network_visibility\": {\n      \"type\": \"string\",\n      \"description\": \"Network accessibility configuration controlling whether\
  \ the cluster is publicly accessible.\",\n      \"enum\": [\"PRIVATE\", \"PUBLIC\"]\n    },\n    \"azure_cluster_identity_client_id\": {\n      \"type\": \"string\",\n      \"description\": \"Client ID of the Azure cluster identity, present for Azure deployments that support CMEK.\"\n    },\n    \"cidr_range\": {\n      \"type\": \"string\",\n      \"description\": \"IPv4 CIDR range reserved for the cluster. Only set on GCP Advanced tier clusters.\",\n      \"pattern\": \"^([0-9]{1,3}\\\\.){3}[0-9]{1,3}/[0-9]{1,2}$\"\n    },\n    \"customer_cloud_account\": {\n      \"$ref\": \"#/$defs/CustomerCloudAccount\",\n      \"description\": \"Customer cloud account details for BYOC (Bring Your Own Cloud) deployments.\"\n    }\n  },\n  \"$defs\": {\n    \"Region\": {\n      \"type\": \"object\",\n      \"description\": \"A geographic region where the cluster or its nodes are deployed.\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Cloud provider region identifier (e.g. us-east-1, us-central1).\"\n        },\n        \"sql_dns\": {\n          \"type\": \"string\",\n          \"description\": \"DNS hostname for SQL connections routed specifically to this region.\"\n        },\n        \"node_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of CockroachDB nodes deployed in this region.\",\n          \"minimum\": 1\n        },\n        \"primary\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is the primary region for a multi-region cluster.\"\n        }\n      }\n    },\n    \"ClusterConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration container for a cluster, holding either serverless or dedicated settings.\",\n      \"properties\": {\n        \"serverless\": {\n          \"$ref\": \"#/$defs/ServerlessClusterConfig\",\n          \"description\": \"Configuration specific to Serverless clusters.\
  \ Present when plan is SERVERLESS.\"\n        },\n        \"dedicated\": {\n          \"$ref\": \"#/$defs/DedicatedClusterConfig\",\n          \"description\": \"Configuration specific to Dedicated clusters. Present when plan is DEDICATED.\"\n        }\n      }\n    },\n    \"ServerlessClusterConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration specific to a CockroachDB Serverless cluster.\",\n      \"properties\": {\n        \"spend_limit\": {\n          \"type\": \"integer\",\n          \"description\": \"Monthly spend limit in US cents. Set to 0 for unlimited spend.\",\n          \"minimum\": 0\n        },\n        \"routing_id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique routing identifier used to route SQL connections to the correct serverless cluster.\"\n        },\n        \"usage_limits\": {\n          \"$ref\": \"#/$defs/UsageLimits\",\n          \"description\": \"Request unit and storage limits for the serverless cluster.\"\
  \n        }\n      }\n    },\n    \"UsageLimits\": {\n      \"type\": \"object\",\n      \"description\": \"Usage-based limits for a Serverless cluster.\",\n      \"properties\": {\n        \"request_unit_limit\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Maximum number of request units per month. 0 means no limit.\"\n        },\n        \"storage_mib_limit\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Maximum storage in mebibytes. 0 means no limit.\"\n        }\n      }\n    },\n    \"DedicatedClusterConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration specific to a CockroachDB Dedicated cluster.\",\n      \"properties\": {\n        \"machine_type\": {\n          \"type\": \"string\",\n          \"description\": \"Machine type used for cluster nodes (e.g. m5.xlarge on AWS).\"\n        },\n        \"num_virtual_cpus\": {\n          \"type\": \"\
  integer\",\n          \"description\": \"Number of virtual CPUs allocated per node.\",\n          \"minimum\": 2\n        },\n        \"storage_gib\": {\n          \"type\": \"integer\",\n          \"description\": \"Storage capacity per node in gibibytes.\",\n          \"minimum\": 15\n        },\n        \"memory_gib\": {\n          \"type\": \"number\",\n          \"description\": \"Memory per node in gibibytes.\",\n          \"exclusiveMinimum\": 0\n        },\n        \"disk_iops\": {\n          \"type\": \"integer\",\n          \"description\": \"Disk input/output operations per second allocated per node.\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"CustomerCloudAccount\": {\n      \"type\": \"object\",\n      \"description\": \"Customer cloud account details for Bring Your Own Cloud (BYOC) cluster deployments.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Cloud provider account or project ID.\"\n\
  \        },\n        \"provider\": {\n          \"type\": \"string\",\n          \"description\": \"Cloud provider for the customer account.\",\n          \"enum\": [\"GCP\", \"AWS\", \"AZURE\"]\n        }\n      }\n    },\n    \"AllowlistEntry\": {\n      \"type\": \"object\",\n      \"description\": \"An IP allowlist entry defining a CIDR range authorized to connect to the cluster.\",\n      \"required\": [\"cidr_ip\", \"cidr_mask\"],\n      \"properties\": {\n        \"cidr_ip\": {\n          \"type\": \"string\",\n          \"description\": \"IPv4 base address of the CIDR range.\",\n          \"pattern\": \"^([0-9]{1,3}\\\\.){3}[0-9]{1,3}$\"\n        },\n        \"cidr_mask\": {\n          \"type\": \"integer\",\n          \"description\": \"Prefix length of the CIDR range (e.g. 24 for /24).\",\n          \"minimum\": 0,\n          \"maximum\": 32\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable label for this allowlist\
  \ entry (e.g. office-network).\"\n        },\n        \"ui\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this entry grants access to the DB Console web interface.\"\n        },\n        \"sql\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this entry grants SQL connection access.\"\n        }\n      }\n    },\n    \"MaintenanceWindow\": {\n      \"type\": \"object\",\n      \"description\": \"Defines the preferred time window for automatic maintenance and version upgrade operations.\",\n      \"properties\": {\n        \"day_of_week\": {\n          \"type\": \"integer\",\n          \"description\": \"Day of the week for the maintenance window. 0=Sunday through 6=Saturday.\",\n          \"minimum\": 0,\n          \"maximum\": 6\n        },\n        \"start_hour\": {\n          \"type\": \"integer\",\n          \"description\": \"Hour of day in UTC when the maintenance window begins (0-23).\",\n          \"minimum\": 0,\n      \
  \    \"maximum\": 23\n        }\n      }\n    },\n    \"CMEKRegionSpec\": {\n      \"type\": \"object\",\n      \"description\": \"Customer-managed encryption key specification for a specific cloud region.\",\n      \"required\": [\"region\", \"key\"],\n      \"properties\": {\n        \"region\": {\n          \"type\": \"string\",\n          \"description\": \"Cloud provider region this key specification applies to.\"\n        },\n        \"key\": {\n          \"$ref\": \"#/$defs/CMEKKeySpec\",\n          \"description\": \"Encryption key specification for this region.\"\n        }\n      }\n    },\n    \"CMEKKeySpec\": {\n      \"type\": \"object\",\n      \"description\": \"Specification for a customer-managed encryption key.\",\n      \"required\": [\"type\", \"uri\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of encryption key. AWS_KMS for AWS, GCP_CLOUD_KMS for GCP.\",\n          \"enum\": [\"AWS_KMS\", \"GCP_CLOUD_KMS\"\
  ]\n        },\n        \"uri\": {\n          \"type\": \"string\",\n          \"description\": \"Full URI of the customer-managed key in the cloud provider's KMS.\"\n        },\n        \"auth_principal\": {\n          \"type\": \"string\",\n          \"description\": \"IAM role ARN (AWS) or service account email (GCP) used to access the key.\"\n        }\n      }\n    },\n    \"LogExportGroup\": {\n      \"type\": \"object\",\n      \"description\": \"A log channel group configuration for selective log export.\",\n      \"required\": [\"channels\"],\n      \"properties\": {\n        \"log_name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the log group or stream in the destination service.\"\n        },\n        \"channels\": {\n          \"type\": \"array\",\n          \"description\": \"List of CockroachDB log channel names to include in this group.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"min_level\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Minimum severity level of log entries to export.\",\n          \"enum\": [\"INFO\", \"WARNING\", \"ERROR\", \"FATAL\"]\n        },\n        \"redact\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to redact sensitive information from log entries before export.\"\n        }\n      }\n    },\n    \"BackupConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Backup retention and frequency settings for a CockroachDB cluster.\",\n      \"properties\": {\n        \"cluster_id\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the cluster this backup configuration applies to.\"\n        },\n        \"frequency_minutes\": {\n          \"type\": \"integer\",\n          \"description\": \"How often automated backups are taken, in minutes.\",\n          \"minimum\": 1\n        },\n        \"retention_days\": {\n          \"type\": \"integer\",\n          \"description\"\
  : \"Number of days automated backups are retained before deletion.\",\n          \"minimum\": 1,\n          \"maximum\": 365\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cockroachdb/refs/heads/main/json-schema/cockroachdb-cluster-schema.json
tags:
- Cluster Management
- Cloud
- Database
- Distributed SQL
- Infrastructure
- PostgreSQL Compatible
- SQL
title: CockroachDB Cluster
---
