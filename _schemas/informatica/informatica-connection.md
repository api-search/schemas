---
description: Schema for an Informatica Intelligent Cloud Services (IICS) connection resource. Connections define the configuration required to access data sources and targets including databases, flat files, cloud applications, and SaaS services through the Platform REST API.
layout: schema
name: Informatica IICS Connection
properties_list:
- description: The resource type identifier for the IICS REST API. Always set to 'connection' for connection resources.
  name: '@type'
  type: string
- description: The unique identifier for the connection, assigned by the platform upon creation.
  name: id
  type: string
- description: The organization ID that owns this connection.
  name: orgId
  type: string
- description: The display name of the connection. Must be unique within the organization. Spaces in the name are encoded as %20 when used in URI paths.
  name: name
  type: string
- description: A human-readable description of the connection and its purpose.
  name: description
  type: string
- description: The connection type that determines which data source or target the connection accesses. Each type requires specific configuration properties.
  name: type
  type: string
- description: The ISO 8601 timestamp when the connection was created.
  name: createTime
  type: string
- description: The ISO 8601 timestamp when the connection was last updated.
  name: updateTime
  type: string
- description: The username of the user who created the connection.
  name: createdBy
  type: string
- description: The username of the user who last updated the connection.
  name: updatedBy
  type: string
- description: The ID of the Secure Agent associated with the connection. The Secure Agent provides the runtime execution environment on-premises or in a private cloud.
  name: agentId
  type: string
- description: The ID of the runtime environment associated with the connection. Determines where connection operations are executed.
  name: runtimeEnvironmentId
  type: string
- description: The hostname or IP address of the data source server. Required for database and server-based connection types such as Oracle, MySQL, and SqlServer.
  name: host
  type: string
- description: The port number for the data source server. Required for database connections.
  name: port
  type: integer
- description: 'The database name, service name, or SID for the connection. The meaning varies by connection type: for Oracle this is the service name or SID, for MySQL and SqlServer this is the database name.'
  name: database
  type: string
- description: The database schema name. Used to narrow the scope of accessible objects within the database.
  name: schema
  type: string
- description: The username for authenticating with the data source.
  name: username
  type: string
- description: The password for authenticating with the data source. This value is write-only and is not returned in GET responses.
  name: password
  type: string
- description: The authentication method used by the connection. Available values depend on the connection type.
  name: authenticationType
  type: string
- description: The service endpoint URL. Required for web service and cloud application connections such as Salesforce, WebServicesConsumer, and TOOLKIT connections.
  name: serviceUrl
  type: string
- description: The character encoding used for the connection. Determines how character data is read from and written to the source or target.
  name: codepage
  type: string
- description: Additional connection parameters specific to the connection type. Contains configuration attributes that are not represented as top-level properties. The available parameters vary by connection type.
  name: connParams
  type: object
provider_name: Informatica
provider_slug: informatica
schema_file: json-schema/informatica-connection-schema.json
slug: informatica-connection
source_json: "{\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/json-schema/informatica-connection-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Informatica IICS Connection\",\n  \"description\": \"Schema for an Informatica Intelligent Cloud Services (IICS) connection resource. Connections define the configuration required to access data sources and targets including databases, flat files, cloud applications, and SaaS services through the Platform REST API.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"type\",\n    \"runtimeEnvironmentId\"\n  ],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"connection\",\n      \"description\": \"The resource type identifier for the IICS REST API. Always set to 'connection' for connection resources.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier\
  \ for the connection, assigned by the platform upon creation.\",\n      \"readOnly\": true\n    },\n    \"orgId\": {\n      \"type\": \"string\",\n      \"description\": \"The organization ID that owns this connection.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the connection. Must be unique within the organization. Spaces in the name are encoded as %20 when used in URI paths.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the connection and its purpose.\",\n      \"maxLength\": 4000\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The connection type that determines which data source or target the connection accesses. Each type requires specific configuration properties.\",\n      \"enum\": [\n        \"CSVFile\",\n        \"FTP\",\n        \"SFTP\"\
  ,\n        \"MS_ACCESS\",\n        \"MSD\",\n        \"MySQL\",\n        \"ODBC\",\n        \"Oracle\",\n        \"OCOD\",\n        \"Salesforce\",\n        \"SqlServer\",\n        \"SqlServer2000\",\n        \"SqlServer2005\",\n        \"SqlServer2008\",\n        \"SqlServer2012\",\n        \"SqlServer2014\",\n        \"SqlServer2016\",\n        \"SqlServer2017\",\n        \"TOOLKIT\",\n        \"WebServicesConsumer\",\n        \"SAP_ALE_IDoc_Reader\",\n        \"SAP_ALE_IDoc_Writer\"\n      ]\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the connection was created.\",\n      \"readOnly\": true\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the connection was last updated.\",\n      \"readOnly\": true\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The username of the user who created the connection.\",\n      \"readOnly\": true\n    },\n    \"updatedBy\": {\n      \"type\": \"string\",\n      \"description\": \"The username of the user who last updated the connection.\",\n      \"readOnly\": true\n    },\n    \"agentId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Secure Agent associated with the connection. The Secure Agent provides the runtime execution environment on-premises or in a private cloud.\"\n    },\n    \"runtimeEnvironmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the runtime environment associated with the connection. Determines where connection operations are executed.\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname or IP address of the data source server. Required for database and server-based connection types such as Oracle, MySQL, and SqlServer.\",\n      \"examples\": [\n        \"db-server.example.com\",\n\
  \        \"192.168.1.100\"\n      ]\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port number for the data source server. Required for database connections.\",\n      \"minimum\": 1,\n      \"maximum\": 65535,\n      \"examples\": [\n        1521,\n        3306,\n        1433\n      ]\n    },\n    \"database\": {\n      \"type\": \"string\",\n      \"description\": \"The database name, service name, or SID for the connection. The meaning varies by connection type: for Oracle this is the service name or SID, for MySQL and SqlServer this is the database name.\",\n      \"examples\": [\n        \"ORCL\",\n        \"mydb\",\n        \"AdventureWorks\"\n      ]\n    },\n    \"schema\": {\n      \"type\": \"string\",\n      \"description\": \"The database schema name. Used to narrow the scope of accessible objects within the database.\",\n      \"examples\": [\n        \"dbo\",\n        \"public\",\n        \"HR\"\n      ]\n    },\n    \"username\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The username for authenticating with the data source.\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"The password for authenticating with the data source. This value is write-only and is not returned in GET responses.\",\n      \"writeOnly\": true\n    },\n    \"authenticationType\": {\n      \"type\": \"string\",\n      \"description\": \"The authentication method used by the connection. Available values depend on the connection type.\",\n      \"examples\": [\n        \"Basic\",\n        \"OAuth2\",\n        \"Kerberos\",\n        \"WindowsAuthentication\"\n      ]\n    },\n    \"serviceUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The service endpoint URL. Required for web service and cloud application connections such as Salesforce, WebServicesConsumer, and TOOLKIT connections.\",\n      \"examples\": [\n        \"https://login.salesforce.com\"\
  ,\n        \"https://api.example.com/service\"\n      ]\n    },\n    \"codepage\": {\n      \"type\": \"string\",\n      \"description\": \"The character encoding used for the connection. Determines how character data is read from and written to the source or target.\",\n      \"default\": \"UTF-8\",\n      \"examples\": [\n        \"UTF-8\",\n        \"ISO-8859-1\",\n        \"MS1252\"\n      ]\n    },\n    \"connParams\": {\n      \"type\": \"object\",\n      \"description\": \"Additional connection parameters specific to the connection type. Contains configuration attributes that are not represented as top-level properties. The available parameters vary by connection type.\",\n      \"additionalProperties\": true,\n      \"examples\": [\n        {\n          \"fetchSize\": \"2000\",\n          \"useSSL\": \"true\",\n          \"truststorePath\": \"/opt/certs/truststore.jks\"\n        }\n      ]\n    }\n  },\n  \"allOf\": [\n    {\n      \"if\": {\n        \"properties\": {\n       \
  \   \"type\": {\n            \"enum\": [\n              \"Oracle\",\n              \"MySQL\",\n              \"SqlServer\",\n              \"SqlServer2000\",\n              \"SqlServer2005\",\n              \"SqlServer2008\",\n              \"SqlServer2012\",\n              \"SqlServer2014\",\n              \"SqlServer2016\",\n              \"SqlServer2017\"\n            ]\n          }\n        },\n        \"required\": [\n          \"type\"\n        ]\n      },\n      \"then\": {\n        \"required\": [\n          \"host\",\n          \"port\",\n          \"database\",\n          \"username\"\n        ]\n      }\n    },\n    {\n      \"if\": {\n        \"properties\": {\n          \"type\": {\n            \"enum\": [\n              \"FTP\",\n              \"SFTP\"\n            ]\n          }\n        },\n        \"required\": [\n          \"type\"\n        ]\n      },\n      \"then\": {\n        \"required\": [\n          \"host\",\n          \"username\"\n        ]\n      }\n    },\n\
  \    {\n      \"if\": {\n        \"properties\": {\n          \"type\": {\n            \"const\": \"Salesforce\"\n          }\n        },\n        \"required\": [\n          \"type\"\n        ]\n      },\n      \"then\": {\n        \"required\": [\n          \"serviceUrl\",\n          \"username\"\n        ]\n      }\n    }\n  ],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/json-schema/informatica-connection-schema.json
tags:
- Address Verification
- B2B Gateway
- Cloud Services
- Data Governance
- Data Integration
- Data Profiling
- Data Quality
- Enterprise Software
- ETL
- IDMC
- IICS
- Master Data Management
- Reference Data Management
title: Informatica IICS Connection
---
