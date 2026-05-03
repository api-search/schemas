---
description: Represents an Oracle Autonomous Database instance in Oracle Cloud Infrastructure, including configuration, lifecycle state, connection details, and scaling parameters.
layout: schema
name: Oracle Autonomous Database
properties_list:
- description: The OCID (Oracle Cloud Identifier) of the Autonomous Database
  name: id
  type: string
- description: The OCID of the compartment containing the Autonomous Database
  name: compartmentId
  type: string
- description: User-friendly display name for the Autonomous Database
  name: displayName
  type: string
- description: The database name, unique within the tenancy
  name: dbName
  type: string
- description: Oracle Database version
  name: dbVersion
  type: string
- description: The workload type of the Autonomous Database
  name: dbWorkload
  type: string
- description: Number of CPU cores allocated
  name: cpuCoreCount
  type: integer
- description: Number of OCPU cores allocated
  name: ocpuCount
  type: number
- description: Data storage size in terabytes
  name: dataStorageSizeInTBs
  type: integer
- description: Data storage size in gigabytes
  name: dataStorageSizeInGBs
  type: integer
- description: Whether auto-scaling is enabled for CPU resources
  name: isAutoScalingEnabled
  type: boolean
- description: Whether auto-scaling is enabled for storage
  name: isAutoScalingForStorageEnabled
  type: boolean
- description: Whether the database runs on dedicated Exadata infrastructure
  name: isDedicated
  type: boolean
- description: Whether this is an Always Free Autonomous Database
  name: isFreeTier
  type: boolean
- description: Current lifecycle state of the Autonomous Database
  name: lifecycleState
  type: string
- description: The Oracle license model for the Autonomous Database
  name: licenseModel
  type: string
- description: Connection strings for different service levels
  name: connectionStrings
  type: object
- description: URLs for database tools and services
  name: connectionUrls
  type: object
- description: List of allowed IP addresses or CIDR blocks for access control
  name: whitelistedIps
  type: array
- description: The OCID of the subnet for private endpoint access
  name: subnetId
  type: string
- description: Private endpoint IP address
  name: privateEndpointIp
  type: string
- description: Private endpoint DNS label
  name: privateEndpointLabel
  type: string
- description: Timestamp when the database was created
  name: timeCreated
  type: string
- description: Start time of next scheduled maintenance window
  name: timeMaintenanceBegin
  type: string
- description: End time of next scheduled maintenance window
  name: timeMaintenanceEnd
  type: string
- description: Free-form tags for resource categorization
  name: freeformTags
  type: object
- description: Defined tags for resource governance
  name: definedTags
  type: object
provider_name: Oracle Database
provider_slug: oracle-database
schema_file: json-schema/oracle-database-autonomous-database.json
slug: oracle-database-autonomous-database
source_filename: oracle-database-autonomous-database.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://oracle.com/schemas/database/autonomous-database.json\",\n  \"title\": \"Oracle Autonomous Database\",\n  \"description\": \"Represents an Oracle Autonomous Database instance in Oracle Cloud Infrastructure, including configuration, lifecycle state, connection details, and scaling parameters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID (Oracle Cloud Identifier) of the Autonomous Database\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the compartment containing the Autonomous Database\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"User-friendly display name for the Autonomous Database\"\n    },\n    \"dbName\": {\n      \"type\": \"string\",\n      \"description\": \"The database name, unique within the tenancy\"\
  ,\n      \"pattern\": \"^[a-zA-Z][a-zA-Z0-9_]{0,13}$\"\n    },\n    \"dbVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Oracle Database version\"\n    },\n    \"dbWorkload\": {\n      \"type\": \"string\",\n      \"description\": \"The workload type of the Autonomous Database\",\n      \"enum\": [\"OLTP\", \"DW\", \"AJD\", \"APEX\"]\n    },\n    \"cpuCoreCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of CPU cores allocated\",\n      \"minimum\": 1\n    },\n    \"ocpuCount\": {\n      \"type\": \"number\",\n      \"description\": \"Number of OCPU cores allocated\"\n    },\n    \"dataStorageSizeInTBs\": {\n      \"type\": \"integer\",\n      \"description\": \"Data storage size in terabytes\",\n      \"minimum\": 1\n    },\n    \"dataStorageSizeInGBs\": {\n      \"type\": \"integer\",\n      \"description\": \"Data storage size in gigabytes\"\n    },\n    \"isAutoScalingEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ auto-scaling is enabled for CPU resources\"\n    },\n    \"isAutoScalingForStorageEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether auto-scaling is enabled for storage\"\n    },\n    \"isDedicated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the database runs on dedicated Exadata infrastructure\"\n    },\n    \"isFreeTier\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is an Always Free Autonomous Database\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle state of the Autonomous Database\",\n      \"enum\": [\n        \"PROVISIONING\",\n        \"AVAILABLE\",\n        \"STOPPING\",\n        \"STOPPED\",\n        \"STARTING\",\n        \"TERMINATING\",\n        \"TERMINATED\",\n        \"UNAVAILABLE\",\n        \"RESTORE_IN_PROGRESS\",\n        \"RESTORE_FAILED\",\n        \"BACKUP_IN_PROGRESS\",\n        \"SCALE_IN_PROGRESS\",\n        \"AVAILABLE_NEEDS_ATTENTION\"\
  ,\n        \"UPDATING\",\n        \"MAINTENANCE_IN_PROGRESS\",\n        \"RESTARTING\",\n        \"RECREATING\",\n        \"ROLE_CHANGE_IN_PROGRESS\",\n        \"UPGRADING\",\n        \"INACCESSIBLE\"\n      ]\n    },\n    \"licenseModel\": {\n      \"type\": \"string\",\n      \"description\": \"The Oracle license model for the Autonomous Database\",\n      \"enum\": [\"LICENSE_INCLUDED\", \"BRING_YOUR_OWN_LICENSE\"]\n    },\n    \"connectionStrings\": {\n      \"type\": \"object\",\n      \"description\": \"Connection strings for different service levels\",\n      \"properties\": {\n        \"high\": {\n          \"type\": \"string\",\n          \"description\": \"High-priority connection string with highest parallelism\"\n        },\n        \"medium\": {\n          \"type\": \"string\",\n          \"description\": \"Medium-priority connection string with moderate parallelism\"\n        },\n        \"low\": {\n          \"type\": \"string\",\n          \"description\": \"Low-priority\
  \ connection string for batch operations\"\n        },\n        \"dedicated\": {\n          \"type\": \"string\",\n          \"description\": \"Connection string for dedicated infrastructure\"\n        }\n      }\n    },\n    \"connectionUrls\": {\n      \"type\": \"object\",\n      \"description\": \"URLs for database tools and services\",\n      \"properties\": {\n        \"sqlDevWebUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for SQL Developer Web\"\n        },\n        \"apexUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for Oracle APEX\"\n        },\n        \"machineLearningUserManagementUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for Machine Learning user management\"\n        },\n        \"graphStudioUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\"\
  : \"URL for Graph Studio\"\n        },\n        \"mongoDbUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for MongoDB API access\"\n        },\n        \"ordsUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for Oracle REST Data Services\"\n        },\n        \"databaseTransformUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for Data Transforms\"\n        }\n      }\n    },\n    \"whitelistedIps\": {\n      \"type\": \"array\",\n      \"description\": \"List of allowed IP addresses or CIDR blocks for access control\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"subnetId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the subnet for private endpoint access\"\n    },\n    \"privateEndpointIp\": {\n      \"type\": \"string\",\n      \"description\": \"Private endpoint\
  \ IP address\"\n    },\n    \"privateEndpointLabel\": {\n      \"type\": \"string\",\n      \"description\": \"Private endpoint DNS label\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the database was created\"\n    },\n    \"timeMaintenanceBegin\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Start time of next scheduled maintenance window\"\n    },\n    \"timeMaintenanceEnd\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"End time of next scheduled maintenance window\"\n    },\n    \"freeformTags\": {\n      \"type\": \"object\",\n      \"description\": \"Free-form tags for resource categorization\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"definedTags\": {\n      \"type\": \"object\",\n      \"description\": \"Defined tags for resource governance\",\n    \
  \  \"additionalProperties\": {\n        \"type\": \"object\"\n      }\n    }\n  },\n  \"required\": [\"id\", \"compartmentId\", \"dbName\", \"lifecycleState\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-database/refs/heads/main/json-schema/oracle-database-autonomous-database.json
tags:
- Cloud
- Database
- Enterprise
- Oracle
- REST API
- SQL
title: Oracle Autonomous Database
---
