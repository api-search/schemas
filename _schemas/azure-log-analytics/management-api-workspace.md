---
description: The top level Log Analytics Workspace resource container.
layout: schema
name: Workspace
properties_list:
- description: Fully qualified resource ID.
  name: id
  type: string
- description: The name of the resource.
  name: name
  type: string
- description: The type of the resource.
  name: type
  type: string
- description: The geo-location where the resource lives.
  name: location
  type: string
- description: Resource tags.
  name: tags
  type: object
- description: The etag of the workspace.
  name: etag
  type: string
- description: Workspace properties.
  name: properties
  type: object
provider_name: Azure Log Analytics
provider_slug: azure-log-analytics
schema_file: json-schema/management-api-workspace-schema.json
slug: management-api-workspace
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/json-schema/management-api-workspace-schema.json\",\n  \"title\": \"Workspace\",\n  \"description\": \"The top level Log Analytics Workspace resource container.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified resource ID.\",\n      \"readOnly\": true,\n      \"example\": \"/subscriptions/00000000-0000-0000-0000-000000000000/resourcegroups/rg1/providers/microsoft.operationalinsights/workspaces/ws1\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the resource.\",\n      \"readOnly\": true,\n      \"example\": \"ws1\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the resource.\",\n      \"readOnly\": true,\n      \"example\": \"Microsoft.OperationalInsights/workspaces\"\
  \n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The geo-location where the resource lives.\",\n      \"example\": \"eastus\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Resource tags.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The etag of the workspace.\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Workspace properties.\",\n      \"properties\": {\n        \"customerId\": {\n          \"type\": \"string\",\n          \"description\": \"Read-only ID associated with the workspace.\",\n          \"readOnly\": true\n        },\n        \"provisioningState\": {\n          \"type\": \"string\",\n          \"description\": \"The provisioning state of the workspace.\",\n          \"enum\": [\"Creating\", \"Succeeded\", \"Failed\", \"Canceled\", \"Deleting\", \"ProvisioningAccount\"\
  , \"Updating\"]\n        },\n        \"sku\": {\n          \"type\": \"object\",\n          \"description\": \"The SKU of the workspace.\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"The name of the SKU.\",\n              \"enum\": [\"Free\", \"Standard\", \"Premium\", \"PerNode\", \"PerGB2018\", \"Standalone\", \"CapacityReservation\", \"LACluster\"]\n            },\n            \"capacityReservationLevel\": {\n              \"type\": \"integer\",\n              \"format\": \"int32\",\n              \"description\": \"The capacity reservation level in GB.\"\n            }\n          }\n        },\n        \"retentionInDays\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\",\n          \"description\": \"The workspace data retention in days.\"\n        },\n        \"publicNetworkAccessForIngestion\": {\n          \"type\": \"string\",\n          \"description\": \"Network access type\
  \ for ingestion.\",\n          \"enum\": [\"Enabled\", \"Disabled\"],\n          \"default\": \"Enabled\"\n        },\n        \"publicNetworkAccessForQuery\": {\n          \"type\": \"string\",\n          \"description\": \"Network access type for query.\",\n          \"enum\": [\"Enabled\", \"Disabled\"],\n          \"default\": \"Enabled\"\n        },\n        \"workspaceCapping\": {\n          \"type\": \"object\",\n          \"description\": \"The daily volume cap for ingestion.\",\n          \"properties\": {\n            \"dailyQuotaGb\": {\n              \"type\": \"number\",\n              \"format\": \"double\",\n              \"description\": \"The workspace daily quota for ingestion in GB.\"\n            },\n            \"dataIngestionStatus\": {\n              \"type\": \"string\",\n              \"description\": \"The status of data ingestion.\",\n              \"enum\": [\"RespectQuota\", \"ForceOn\", \"ForceOff\", \"OverQuota\", \"SubscriptionSuspended\", \"ApproachingQuota\"\
  ]\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/json-schema/management-api-workspace-schema.json
tags:
- Analytics
- Azure
- Cloud
- Logging
- Monitoring
title: Workspace
---
