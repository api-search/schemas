---
description: A data source connection in Oracle Essbase used for data loading and dimension building operations. Connections can be defined at the application level or globally. They store the configuration required to connect to external databases and data sources such as Oracle, SQL Server, and file-based sources.
layout: schema
name: Oracle Essbase Connection
properties_list:
- description: Connection name used to reference this connection in jobs and scripts.
  name: name
  type: string
- description: Human-readable description of the connection purpose and target.
  name: description
  type: string
- description: Connection type identifying the target data source technology (e.g., Oracle, SQL Server, file-based).
  name: type
  type: string
- description: Database host address or server name.
  name: host
  type: string
- description: Database port number for the connection.
  name: port
  type: integer
- description: Database service name or SID for Oracle connections.
  name: serviceName
  type: string
- description: Database username for authentication.
  name: user
  type: string
- description: Database password for authentication. Write-only; not returned in API responses.
  name: password
  type: string
- description: Path to the Oracle wallet file for secure SSL/TLS connections.
  name: walletPath
  type: string
- description: HATEOAS navigation links.
  name: links
  type: array
provider_name: Oracle Essbase
provider_slug: oracle-essbase
schema_file: json-schema/oracle-essbase-connection-schema.json
slug: oracle-essbase-connection
source_filename: oracle-essbase-connection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"oracle-essbase-connection-schema.json\",\n  \"title\": \"Oracle Essbase Connection\",\n  \"description\": \"A data source connection in Oracle Essbase used for data loading and dimension building operations. Connections can be defined at the application level or globally. They store the configuration required to connect to external databases and data sources such as Oracle, SQL Server, and file-based sources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Connection name used to reference this connection in jobs and scripts.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the connection purpose and target.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Connection type identifying the target data source technology (e.g.,\
  \ Oracle, SQL Server, file-based).\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Database host address or server name.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"Database port number for the connection.\"\n    },\n    \"serviceName\": {\n      \"type\": \"string\",\n      \"description\": \"Database service name or SID for Oracle connections.\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"Database username for authentication.\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Database password for authentication. Write-only; not returned in API responses.\"\n    },\n    \"walletPath\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the Oracle wallet file for secure SSL/TLS connections.\"\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"description\": \"HATEOAS navigation links.\",\n      \"items\": {\n        \"\
  $ref\": \"#/$defs/Link\"\n      }\n    }\n  },\n  \"required\": [\"name\", \"type\"],\n  \"$defs\": {\n    \"Link\": {\n      \"type\": \"object\",\n      \"description\": \"HATEOAS navigation link.\",\n      \"properties\": {\n        \"rel\": {\n          \"type\": \"string\",\n          \"description\": \"Link relation type.\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Link URL.\"\n        },\n        \"method\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP method for this link.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Media type of the linked resource.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-essbase/refs/heads/main/json-schema/oracle-essbase-connection-schema.json
tags:
- Analytics
- Budgeting
- Business Intelligence
- Financial Consolidation
- Multi-Dimensional Database
- OLAP
- Planning
title: Oracle Essbase Connection
---
