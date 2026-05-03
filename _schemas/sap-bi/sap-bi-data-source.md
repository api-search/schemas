---
description: A data source connection used across SAP BI products to connect to source systems, databases, cloud services, and other data repositories for analytics and reporting.
layout: schema
name: SAP BI Data Source
properties_list:
- description: Data source unique identifier
  name: id
  type: string
- description: Data source name
  name: name
  type: string
- description: Data source description
  name: description
  type: string
- description: Connection type indicating the source system
  name: type
  type: string
- description: Current connection status
  name: status
  type: string
- description: Hostname or endpoint URL of the data source
  name: host
  type: string
- description: Connection port number
  name: port
  type: integer
- description: Database or schema name
  name: database
  type: string
- description: Authentication method used for the connection
  name: authenticationMethod
  type: string
- description: Whether SSL/TLS encryption is enabled
  name: sslEnabled
  type: boolean
- description: Datasphere space containing this connection
  name: spaceId
  type: string
- description: User who created the data source
  name: createdBy
  type: string
- description: When the data source was created
  name: createdTime
  type: string
- description: When the data source was last modified
  name: modifiedTime
  type: string
- description: When the connection was last tested
  name: lastTestedTime
  type: string
- description: Result of the last connection test
  name: lastTestResult
  type: string
provider_name: SAP Business Intelligence
provider_slug: sap-bi
schema_file: json-schema/sap-bi-data-source-schema.json
slug: sap-bi-data-source
source_filename: sap-bi-data-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.sap.com/schemas/sap-bi/data-source.json\",\n  \"title\": \"SAP BI Data Source\",\n  \"description\": \"A data source connection used across SAP BI products to connect to source systems, databases, cloud services, and other data repositories for analytics and reporting.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Data source unique identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Data source name\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Data source description\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"HANA\",\n        \"S4HANA\",\n        \"SAP_BW\",\n        \"SAP_BW4HANA\",\n        \"\
  ABAP_CDS\",\n        \"OData\",\n        \"Cloud_Data_Integration\",\n        \"Google_BigQuery\",\n        \"Microsoft_SQL_Server\",\n        \"Amazon_S3\",\n        \"JDBC\",\n        \"File\"\n      ],\n      \"description\": \"Connection type indicating the source system\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Active\", \"Inactive\", \"Error\"],\n      \"description\": \"Current connection status\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname or endpoint URL of the data source\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 65535,\n      \"description\": \"Connection port number\"\n    },\n    \"database\": {\n      \"type\": \"string\",\n      \"description\": \"Database or schema name\"\n    },\n    \"authenticationMethod\": {\n      \"type\": \"string\",\n      \"enum\": [\"BasicAuth\", \"OAuth2\", \"SAML\", \"Kerberos\", \"Certificate\", \"APIKey\"\
  ],\n      \"description\": \"Authentication method used for the connection\"\n    },\n    \"sslEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether SSL/TLS encryption is enabled\"\n    },\n    \"spaceId\": {\n      \"type\": \"string\",\n      \"description\": \"Datasphere space containing this connection\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"User who created the data source\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the data source was created\"\n    },\n    \"modifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the data source was last modified\"\n    },\n    \"lastTestedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the connection was last tested\"\n    },\n    \"lastTestResult\": {\n      \"type\": \"string\",\n\
  \      \"enum\": [\"Success\", \"Failed\"],\n      \"description\": \"Result of the last connection test\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-bi/refs/heads/main/json-schema/sap-bi-data-source-schema.json
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Reporting
- SAP
title: SAP BI Data Source
---
