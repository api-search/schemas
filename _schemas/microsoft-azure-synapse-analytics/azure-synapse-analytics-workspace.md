---
description: A Synapse workspace resource that provides an enterprise analytics environment combining SQL, Spark, and data integration capabilities.
layout: schema
name: Azure Synapse Analytics Workspace
properties_list:
- description: Fully qualified resource ID for the workspace.
  name: id
  type: string
- description: The name of the workspace resource.
  name: name
  type: string
- description: The type of the resource (Microsoft.Synapse/workspaces).
  name: type
  type: string
- description: The geo-location where the workspace resource lives.
  name: location
  type: string
- description: Resource tags for categorization and billing.
  name: tags
  type: object
- description: ''
  name: identity
  type: object
- description: ''
  name: properties
  type: object
provider_name: Azure Synapse Analytics
provider_slug: microsoft-azure-synapse-analytics
schema_file: json-schema/azure-synapse-analytics-workspace-schema.json
slug: azure-synapse-analytics-workspace
source_filename: azure-synapse-analytics-workspace-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/azure-synapse-analytics/json-schema/azure-synapse-analytics-workspace-schema.json\",\n  \"title\": \"Azure Synapse Analytics Workspace\",\n  \"description\": \"A Synapse workspace resource that provides an enterprise analytics environment combining SQL, Spark, and data integration capabilities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified resource ID for the workspace.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workspace resource.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the resource (Microsoft.Synapse/workspaces).\",\n      \"readOnly\": true\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The geo-location\
  \ where the workspace resource lives.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Resource tags for categorization and billing.\"\n    },\n    \"identity\": {\n      \"$ref\": \"#/$defs/ManagedIdentity\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"defaultDataLakeStorage\": {\n          \"$ref\": \"#/$defs/DataLakeStorageAccountDetails\"\n        },\n        \"sqlAdministratorLogin\": {\n          \"type\": \"string\",\n          \"description\": \"Login name for the workspace SQL active directory administrator.\"\n        },\n        \"sqlAdministratorLoginPassword\": {\n          \"type\": \"string\",\n          \"description\": \"SQL administrator login password.\"\n        },\n        \"managedResourceGroupName\": {\n          \"type\": \"string\",\n          \"description\": \"Workspace managed resource group name.\"\n\
  \        },\n        \"provisioningState\": {\n          \"type\": \"string\",\n          \"description\": \"Resource provisioning state.\",\n          \"readOnly\": true\n        },\n        \"connectivityEndpoints\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Connectivity endpoints (SQL, SQL on-demand, dev, web).\",\n          \"readOnly\": true\n        },\n        \"managedVirtualNetwork\": {\n          \"type\": \"string\",\n          \"description\": \"Setting this to 'default' ensures all compute is in a managed virtual network.\"\n        },\n        \"managedVirtualNetworkSettings\": {\n          \"$ref\": \"#/$defs/ManagedVirtualNetworkSettings\"\n        },\n        \"encryption\": {\n          \"$ref\": \"#/$defs/EncryptionDetails\"\n        },\n        \"publicNetworkAccess\": {\n          \"type\": \"string\",\n          \"description\": \"Enable or disable public\
  \ network access to the workspace.\",\n          \"enum\": [\"Enabled\", \"Disabled\"]\n        },\n        \"workspaceUID\": {\n          \"type\": \"string\",\n          \"description\": \"The workspace unique identifier.\",\n          \"readOnly\": true\n        }\n      }\n    }\n  },\n  \"required\": [\"location\"],\n  \"$defs\": {\n    \"ManagedIdentity\": {\n      \"type\": \"object\",\n      \"description\": \"The workspace managed identity configuration.\",\n      \"properties\": {\n        \"principalId\": {\n          \"type\": \"string\",\n          \"description\": \"The principal ID of the workspace managed identity.\",\n          \"readOnly\": true\n        },\n        \"tenantId\": {\n          \"type\": \"string\",\n          \"description\": \"The tenant ID of the workspace managed identity.\",\n          \"readOnly\": true\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of managed identity.\",\n          \"enum\"\
  : [\"None\", \"SystemAssigned\", \"SystemAssigned,UserAssigned\"]\n        }\n      }\n    },\n    \"DataLakeStorageAccountDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Details of the default data lake storage account associated with the workspace.\",\n      \"properties\": {\n        \"accountUrl\": {\n          \"type\": \"string\",\n          \"description\": \"Account URL of the data lake storage.\"\n        },\n        \"filesystem\": {\n          \"type\": \"string\",\n          \"description\": \"Filesystem name in the data lake storage.\"\n        },\n        \"resourceId\": {\n          \"type\": \"string\",\n          \"description\": \"ARM resource ID of the storage account.\"\n        },\n        \"createManagedPrivateEndpoint\": {\n          \"type\": \"boolean\",\n          \"description\": \"Create managed private endpoint to this storage account.\"\n        }\n      }\n    },\n    \"ManagedVirtualNetworkSettings\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"Managed virtual network settings for the workspace.\",\n      \"properties\": {\n        \"preventDataExfiltration\": {\n          \"type\": \"boolean\",\n          \"description\": \"Prevent data exfiltration from the workspace.\"\n        },\n        \"linkedAccessCheckOnTargetResource\": {\n          \"type\": \"boolean\",\n          \"description\": \"Check linked access on target resource.\"\n        },\n        \"allowedAadTenantIdsForLinking\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Allowed AAD Tenant IDs for linking.\"\n        }\n      }\n    },\n    \"EncryptionDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Workspace encryption configuration details.\",\n      \"properties\": {\n        \"cmk\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"key\": {\n              \"type\": \"object\",\n              \"\
  properties\": {\n                \"name\": {\n                  \"type\": \"string\",\n                  \"description\": \"Workspace key name.\"\n                },\n                \"keyVaultUrl\": {\n                  \"type\": \"string\",\n                  \"description\": \"Workspace key sub-resource key vault URL.\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-synapse-analytics/refs/heads/main/json-schema/azure-synapse-analytics-workspace-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Integration
- Data Warehouse
- ETL
- SQL
title: Azure Synapse Analytics Workspace
---
