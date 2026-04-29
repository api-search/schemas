---
description: SourceFlowConfig schema from Amazon AppFlow API
layout: schema
name: SourceFlowConfig
properties_list:
- description: The type of connector used as a source.
  name: connectorType
  type: string
- description: The API version of the connector used in the source.
  name: apiVersion
  type: string
- description: The name of the connector profile. Required for all connectors except Amplitude, Datadog, Dynatrace, GoogleAnalytics, Marketo, SAPOData, Salesforce, ServiceNow, Singular, Slack, Trendmicro, and Veeva.
  name: connectorProfileName
  type: string
- description: Specifies the information that is required to query a particular source connector.
  name: sourceConnectorProperties
  type: object
- description: Defines the configuration for a scheduled incremental data pull. If a valid configuration is provided, the fields specified in the configuration are used when querying for the incremental data pull.
  name: incrementalPullConfig
  type: object
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-source-flow-config-schema.json
slug: appflow-source-flow-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-source-flow-config-schema.json\",\n  \"title\": \"SourceFlowConfig\",\n  \"description\": \"SourceFlowConfig schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorType\": {\n      \"type\": \"string\",\n      \"example\": \"Salesforce\",\n      \"description\": \"The type of connector used as a source.\"\n    },\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"example\": \"v55.0\",\n      \"description\": \"The API version of the connector used in the source.\"\n    },\n    \"connectorProfileName\": {\n      \"type\": \"string\",\n      \"example\": \"my-salesforce-profile\",\n      \"description\": \"The name of the connector profile. Required for all connectors except Amplitude, Datadog, Dynatrace, GoogleAnalytics, Marketo, SAPOData, Salesforce,\
  \ ServiceNow, Singular, Slack, Trendmicro, and Veeva.\"\n    },\n    \"sourceConnectorProperties\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"Salesforce\": {\n          \"object\": \"Account\"\n        }\n      },\n      \"description\": \"Specifies the information that is required to query a particular source connector.\"\n    },\n    \"incrementalPullConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"datetimeTypeFieldName\": {\n          \"type\": \"string\",\n          \"example\": \"LastModifiedDate\",\n          \"description\": \"A field that specifies the date time or timestamp field as the criteria to use when importing incremental records from the source.\"\n        }\n      },\n      \"description\": \"Defines the configuration for a scheduled incremental data pull. If a valid configuration is provided, the fields specified in the configuration are used when querying for the incremental data pull.\"\n    }\n  },\n  \"required\"\
  : [\n    \"connectorType\",\n    \"sourceConnectorProperties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-source-flow-config-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: SourceFlowConfig
---
