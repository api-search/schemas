---
description: Schema for a Power BI dataset resource as returned by the Power BI REST API. A dataset represents the data model that underpins reports and dashboards, including tables, columns, measures, relationships, and data source configuration.
layout: schema
name: Power BI Dataset
properties_list:
- description: The unique identifier of the dataset, assigned by the Power BI service
  name: id
  type: string
- description: The display name of the dataset
  name: name
  type: string
- description: Whether the dataset supports the push rows API for real-time data ingestion
  name: addRowsAPIEnabled
  type: boolean
- description: The email address of the user who configured or last modified the dataset
  name: configuredBy
  type: string
- description: Whether the dataset supports scheduled or on-demand refresh
  name: isRefreshable
  type: boolean
- description: Whether an effective identity (row-level security identity) is required when generating embed tokens
  name: isEffectiveIdentityRequired
  type: boolean
- description: Whether RLS role specification is required in effective identity for embed tokens
  name: isEffectiveIdentityRolesRequired
  type: boolean
- description: Whether the dataset requires an on-premises data gateway to connect to its data sources
  name: isOnPremGatewayRequired
  type: boolean
- description: The storage mode that determines how data is stored and queried
  name: targetStorageMode
  type: string
- description: The default mode for push datasets
  name: defaultMode
  type: string
- description: The UTC date and time when the dataset was first created
  name: createdDate
  type: string
- description: The type of content provider that generated this dataset
  name: contentProviderType
  type: string
- description: The URL to create an embedded report connected to this dataset
  name: createReportEmbedURL
  type: string
- description: The URL for the Q&A natural language embedded experience
  name: qnaEmbedURL
  type: string
- description: The web URL for accessing the dataset in the Power BI service
  name: webUrl
  type: string
- description: The tables that make up the dataset schema
  name: tables
  type: array
- description: The relationships between tables in the dataset model
  name: relationships
  type: array
- description: The data sources used by the dataset
  name: datasources
  type: array
provider_name: Power BI
provider_slug: power-bi
schema_file: json-schema/power-bi-dataset-schema.json
slug: power-bi-dataset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://learn.microsoft.com/schemas/power-bi/dataset.json\",\n  \"title\": \"Power BI Dataset\",\n  \"description\": \"Schema for a Power BI dataset resource as returned by the Power BI REST API. A dataset represents the data model that underpins reports and dashboards, including tables, columns, measures, relationships, and data source configuration.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"tables\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the dataset, assigned by the Power BI service\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the dataset\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n    \"addRowsAPIEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the dataset supports the\
  \ push rows API for real-time data ingestion\",\n      \"default\": false\n    },\n    \"configuredBy\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the user who configured or last modified the dataset\"\n    },\n    \"isRefreshable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the dataset supports scheduled or on-demand refresh\",\n      \"default\": false\n    },\n    \"isEffectiveIdentityRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether an effective identity (row-level security identity) is required when generating embed tokens\",\n      \"default\": false\n    },\n    \"isEffectiveIdentityRolesRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether RLS role specification is required in effective identity for embed tokens\",\n      \"default\": false\n    },\n    \"isOnPremGatewayRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the dataset requires\
  \ an on-premises data gateway to connect to its data sources\",\n      \"default\": false\n    },\n    \"targetStorageMode\": {\n      \"type\": \"string\",\n      \"description\": \"The storage mode that determines how data is stored and queried\",\n      \"enum\": [\"Import\", \"DirectQuery\", \"Dual\", \"PushDataset\"]\n    },\n    \"defaultMode\": {\n      \"type\": \"string\",\n      \"description\": \"The default mode for push datasets\",\n      \"enum\": [\"Push\", \"Streaming\", \"PushStreaming\"]\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The UTC date and time when the dataset was first created\"\n    },\n    \"contentProviderType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of content provider that generated this dataset\"\n    },\n    \"createReportEmbedURL\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to create an embedded report\
  \ connected to this dataset\"\n    },\n    \"qnaEmbedURL\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL for the Q&A natural language embedded experience\"\n    },\n    \"webUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The web URL for accessing the dataset in the Power BI service\"\n    },\n    \"tables\": {\n      \"type\": \"array\",\n      \"description\": \"The tables that make up the dataset schema\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/Table\"\n      }\n    },\n    \"relationships\": {\n      \"type\": \"array\",\n      \"description\": \"The relationships between tables in the dataset model\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Relationship\"\n      }\n    },\n    \"datasources\": {\n      \"type\": \"array\",\n      \"description\": \"The data sources used by the dataset\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Datasource\"\
  \n      }\n    }\n  },\n  \"$defs\": {\n    \"Table\": {\n      \"type\": \"object\",\n      \"description\": \"A table in the Power BI dataset model, containing columns, measures, and optionally rows for push datasets\",\n      \"required\": [\"name\", \"columns\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the table, used in DAX expressions and API references\",\n          \"minLength\": 1,\n          \"maxLength\": 256\n        },\n        \"columns\": {\n          \"type\": \"array\",\n          \"description\": \"The columns defined in this table\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/$defs/Column\"\n          }\n        },\n        \"rows\": {\n          \"type\": \"array\",\n          \"description\": \"Data rows in the table (used for push datasets)\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        },\n        \"measures\": {\n\
  \          \"type\": \"array\",\n          \"description\": \"DAX measures defined on this table\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Measure\"\n          }\n        },\n        \"isHidden\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the table is hidden from report authors\",\n          \"default\": false\n        }\n      }\n    },\n    \"Column\": {\n      \"type\": \"object\",\n      \"description\": \"A column in a dataset table\",\n      \"required\": [\"name\", \"dataType\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The column name used in DAX expressions\",\n          \"minLength\": 1,\n          \"maxLength\": 256\n        },\n        \"dataType\": {\n          \"type\": \"string\",\n          \"description\": \"The data type of the column values\",\n          \"enum\": [\"Int64\", \"Double\", \"Boolean\", \"Datetime\", \"String\", \"Decimal\"]\n        },\n\
  \        \"formatString\": {\n          \"type\": \"string\",\n          \"description\": \"A format string controlling how column values are displayed (e.g. '#,##0.00' for numbers)\"\n        },\n        \"sortByColumn\": {\n          \"type\": \"string\",\n          \"description\": \"The name of another column used to sort this column's values\"\n        },\n        \"dataCategory\": {\n          \"type\": \"string\",\n          \"description\": \"The data category providing semantic meaning to the column (e.g. Address, City, Country)\"\n        },\n        \"isHidden\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the column is hidden from report authors\",\n          \"default\": false\n        },\n        \"summarizeBy\": {\n          \"type\": \"string\",\n          \"description\": \"The default aggregation function for the column\",\n          \"enum\": [\"sum\", \"count\", \"distinctCount\", \"min\", \"max\", \"average\", \"none\"]\n        }\n  \
  \    }\n    },\n    \"Measure\": {\n      \"type\": \"object\",\n      \"description\": \"A DAX measure defined on a dataset table\",\n      \"required\": [\"name\", \"expression\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the measure\",\n          \"minLength\": 1,\n          \"maxLength\": 256\n        },\n        \"expression\": {\n          \"type\": \"string\",\n          \"description\": \"The DAX expression that defines the measure calculation\",\n          \"minLength\": 1\n        },\n        \"formatString\": {\n          \"type\": \"string\",\n          \"description\": \"A format string controlling how the measure value is displayed\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A description of what the measure calculates\"\n        },\n        \"isHidden\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether\
  \ the measure is hidden from report authors\",\n          \"default\": false\n        }\n      }\n    },\n    \"Relationship\": {\n      \"type\": \"object\",\n      \"description\": \"A relationship between two tables in the dataset model\",\n      \"required\": [\"name\", \"fromTable\", \"fromColumn\", \"toTable\", \"toColumn\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The unique name of the relationship\"\n        },\n        \"fromTable\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the source (many-side) table\"\n        },\n        \"fromColumn\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the column in the source table\"\n        },\n        \"toTable\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the target (one-side) table\"\n        },\n        \"toColumn\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The name of the column in the target table\"\n        },\n        \"crossFilteringBehavior\": {\n          \"type\": \"string\",\n          \"description\": \"The cross-filtering direction for the relationship\",\n          \"enum\": [\"OneDirection\", \"BothDirections\", \"Automatic\"],\n          \"default\": \"OneDirection\"\n        }\n      }\n    },\n    \"Datasource\": {\n      \"type\": \"object\",\n      \"description\": \"A data source used by the dataset\",\n      \"properties\": {\n        \"datasourceType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of data source (e.g. Sql, AnalysisServices, File, Web)\"\n        },\n        \"connectionDetails\": {\n          \"type\": \"object\",\n          \"description\": \"Connection details for the data source\",\n          \"properties\": {\n            \"server\": {\n              \"type\": \"string\",\n              \"description\": \"The server address\"\n            },\n            \"database\"\
  : {\n              \"type\": \"string\",\n              \"description\": \"The database name\"\n            },\n            \"url\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"The connection URL for web-based data sources\"\n            },\n            \"path\": {\n              \"type\": \"string\",\n              \"description\": \"The file path for file-based data sources\"\n            }\n          }\n        },\n        \"datasourceId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the bound data source\"\n        },\n        \"gatewayId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The gateway identifier if using an on-premises data gateway\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/json-schema/power-bi-dataset-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
title: Power BI Dataset
---
