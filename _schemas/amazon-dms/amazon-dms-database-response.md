---
description: Describes a database in a Fleet Advisor collector inventory.
layout: schema
name: DatabaseResponse
properties_list:
- description: ''
  name: DatabaseId
  type: object
- description: ''
  name: DatabaseName
  type: object
- description: ''
  name: IpAddress
  type: object
- description: ''
  name: NumberOfSchemas
  type: object
- description: ''
  name: Server
  type: object
- description: ''
  name: SoftwareDetails
  type: object
- description: ''
  name: Collectors
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-database-response-schema.json
slug: amazon-dms-database-response
source_filename: amazon-dms-database-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-database-response-schema.json\",\n  \"title\": \"DatabaseResponse\",\n  \"description\": \"Describes a database in a Fleet Advisor collector inventory.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatabaseId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ID of a database in a Fleet Advisor collector inventory.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of a database in a Fleet Advisor collector inventory. \"\n        }\n      ]\n    },\n    \"IpAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"The IP address of a database in a Fleet Advisor collector inventory. \"\n        }\n      ]\n    },\n    \"NumberOfSchemas\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongOptional\"\n        },\n        {\n          \"description\": \"The number of schemas in a Fleet Advisor collector inventory database. \"\n        }\n      ]\n    },\n    \"Server\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServerShortInfoResponse\"\n        },\n        {\n          \"description\": \"The server name of a database in a Fleet Advisor collector inventory. \"\n        }\n      ]\n    },\n    \"SoftwareDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatabaseInstanceSoftwareDetailsResponse\"\n        },\n        {\n          \"description\": \"The software details of a database in a Fleet Advisor collector inventory, such as database engine and\
  \ version.\"\n        }\n      ]\n    },\n    \"Collectors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CollectorsList\"\n        },\n        {\n          \"description\": \"A list of collectors associated with the database.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-database-response-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: DatabaseResponse
---
