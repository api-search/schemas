---
description: A Power BI dataset representing a data model
layout: schema
name: Dataset
properties_list:
- description: The unique identifier of the dataset
  name: id
  type: string
- description: The display name of the dataset
  name: name
  type: string
- description: Whether the push API is enabled for this dataset
  name: addRowsAPIEnabled
  type: boolean
- description: The user who configured the dataset
  name: configuredBy
  type: string
- description: Whether the dataset can be refreshed
  name: isRefreshable
  type: boolean
- description: Whether effective identity is required for embedding
  name: isEffectiveIdentityRequired
  type: boolean
- description: Whether RLS roles are required for embedding
  name: isEffectiveIdentityRolesRequired
  type: boolean
- description: Whether an on-premises gateway is required
  name: isOnPremGatewayRequired
  type: boolean
- description: The storage mode of the dataset
  name: targetStorageMode
  type: string
- description: URL to create an embedded report on this dataset
  name: createReportEmbedURL
  type: string
- description: URL for the Q&A embedded experience
  name: qnaEmbedURL
  type: string
- description: The web URL of the dataset
  name: webUrl
  type: string
- description: The date and time the dataset was created
  name: createdDate
  type: string
- description: The content provider type
  name: contentProviderType
  type: string
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-rest-dataset-schema.json
slug: power-bi-rest-dataset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Dataset\",\n  \"type\": \"object\",\n  \"description\": \"A Power BI dataset representing a data model\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the dataset\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the dataset\"\n    },\n    \"addRowsAPIEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the push API is enabled for this dataset\"\n    },\n    \"configuredBy\": {\n      \"type\": \"string\",\n      \"description\": \"The user who configured the dataset\"\n    },\n    \"isRefreshable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the dataset can be refreshed\"\n    },\n    \"isEffectiveIdentityRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether effective identity is required for embedding\"\
  \n    },\n    \"isEffectiveIdentityRolesRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether RLS roles are required for embedding\"\n    },\n    \"isOnPremGatewayRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether an on-premises gateway is required\"\n    },\n    \"targetStorageMode\": {\n      \"type\": \"string\",\n      \"description\": \"The storage mode of the dataset\"\n    },\n    \"createReportEmbedURL\": {\n      \"type\": \"string\",\n      \"description\": \"URL to create an embedded report on this dataset\"\n    },\n    \"qnaEmbedURL\": {\n      \"type\": \"string\",\n      \"description\": \"URL for the Q&A embedded experience\"\n    },\n    \"webUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The web URL of the dataset\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the dataset was created\"\n    },\n    \"contentProviderType\": {\n      \"type\":\
  \ \"string\",\n      \"description\": \"The content provider type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-rest-dataset-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: Dataset
---
