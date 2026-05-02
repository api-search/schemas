---
description: Represents a registered data source in the Microsoft Purview scanning service. Data sources are the foundation for automated scanning and data discovery.
layout: schema
name: Microsoft Purview Data Source
properties_list:
- description: The resource identifier of the data source
  name: id
  type: string
- description: The name of the data source
  name: name
  type: string
- description: The type of data source
  name: kind
  type: string
- description: Data source properties specific to its kind
  name: properties
  type: object
provider_name: Microsoft Purview
provider_slug: microsoft-purview
schema_file: json-schema/microsoft-purview-data-source-schema.json
slug: microsoft-purview-data-source
source_filename: microsoft-purview-data-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/microsoft-purview/json-schema/microsoft-purview-data-source-schema.json\",\n  \"title\": \"Microsoft Purview Data Source\",\n  \"description\": \"Represents a registered data source in the Microsoft Purview scanning service. Data sources are the foundation for automated scanning and data discovery.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The resource identifier of the data source\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the data source\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The type of data source\",\n      \"enum\": [\n        \"AzureSubscription\",\n        \"AzureResourceGroup\",\n        \"AzureSynapseWorkspace\",\n        \"AzureSynapse\",\n        \"AdlsGen1\"\
  ,\n        \"AdlsGen2\",\n        \"AmazonAccount\",\n        \"AmazonS3\",\n        \"AmazonSql\",\n        \"AzureCosmosDb\",\n        \"AzureDataExplorer\",\n        \"AzureFileService\",\n        \"AzureSqlDatabase\",\n        \"AzureSqlDatabaseManagedInstance\",\n        \"AzureSqlDataWarehouse\",\n        \"AzureMySql\",\n        \"AzurePostgreSql\",\n        \"AzureStorage\",\n        \"Teradata\",\n        \"Oracle\",\n        \"SapS4Hana\",\n        \"SapEcc\",\n        \"PowerBI\"\n      ]\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Data source properties specific to its kind\",\n      \"properties\": {\n        \"endpoint\": {\n          \"type\": \"string\",\n          \"description\": \"The endpoint URL of the data source\"\n        },\n        \"resourceGroup\": {\n          \"type\": \"string\",\n          \"description\": \"The Azure resource group\"\n        },\n        \"subscriptionId\": {\n          \"type\": \"string\",\n \
  \         \"format\": \"uuid\",\n          \"description\": \"The Azure subscription ID\"\n        },\n        \"location\": {\n          \"type\": \"string\",\n          \"description\": \"The geographic location of the data source\"\n        },\n        \"resourceName\": {\n          \"type\": \"string\",\n          \"description\": \"The Azure resource name\"\n        },\n        \"resourceId\": {\n          \"type\": \"string\",\n          \"description\": \"The Azure resource ID\"\n        },\n        \"collection\": {\n          \"type\": \"object\",\n          \"description\": \"The collection reference\",\n          \"properties\": {\n            \"referenceName\": {\n              \"type\": \"string\"\n            },\n            \"type\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The creation date\"\n        },\n  \
  \      \"lastModifiedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The last modification date\"\n        }\n      }\n    }\n  },\n  \"required\": [\"name\", \"kind\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/json-schema/microsoft-purview-data-source-schema.json
tags:
- Compliance
- Data Catalog
- Data Classification
- Data Governance
- Data Loss Prevention
- Information Protection
title: Microsoft Purview Data Source
---
