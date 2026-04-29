---
description: Specifies a connector to an Amazon Athena data source.
layout: schema
name: AthenaConnectorSource
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: ConnectionName
  type: object
- description: ''
  name: ConnectorName
  type: object
- description: ''
  name: ConnectionType
  type: object
- description: ''
  name: ConnectionTable
  type: object
- description: ''
  name: SchemaName
  type: object
- description: ''
  name: OutputSchemas
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-athena-connector-source-schema.json
slug: glue-athena-connector-source
source_filename: glue-athena-connector-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-athena-connector-source-schema.json\",\n  \"title\": \"AthenaConnectorSource\",\n  \"description\": \"Specifies a connector to an Amazon Athena data source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeName\"\n        },\n        {\n          \"description\": \"The name of the data source.\"\n        }\n      ]\n    },\n    \"ConnectionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnclosedInStringProperty\"\n        },\n        {\n          \"description\": \"The name of the connection that is associated with the connector.\"\n        }\n      ]\n    },\n    \"ConnectorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnclosedInStringProperty\"\
  \n        },\n        {\n          \"description\": \"The name of a connector that assists with accessing the data store in Glue Studio.\"\n        }\n      ]\n    },\n    \"ConnectionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnclosedInStringProperty\"\n        },\n        {\n          \"description\": \"The type of connection, such as marketplace.athena or custom.athena, designating a connection to an Amazon Athena data store.\"\n        }\n      ]\n    },\n    \"ConnectionTable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnclosedInStringPropertyWithQuote\"\n        },\n        {\n          \"description\": \"The name of the table in the data source.\"\n        }\n      ]\n    },\n    \"SchemaName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnclosedInStringProperty\"\n        },\n        {\n          \"description\": \"The name of the Cloudwatch log group to read from. For\
  \ example, <code>/aws-glue/jobs/output</code>.\"\n        }\n      ]\n    },\n    \"OutputSchemas\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueSchemas\"\n        },\n        {\n          \"description\": \"Specifies the data schema for the custom Athena source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"ConnectionName\",\n    \"ConnectorName\",\n    \"ConnectionType\",\n    \"SchemaName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-athena-connector-source-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: AthenaConnectorSource
---
