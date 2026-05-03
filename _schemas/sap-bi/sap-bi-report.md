---
description: A report document in SAP BusinessObjects BI Platform, representing Crystal Reports, Web Intelligence documents, or publications managed through the content management system.
layout: schema
name: SAP BusinessObjects Report
properties_list:
- description: Report unique system identifier (SI_ID)
  name: id
  type: integer
- description: Cluster unique identifier (SI_CUID)
  name: cuid
  type: string
- description: Report name
  name: name
  type: string
- description: Report description
  name: description
  type: string
- description: Report type indicating the reporting engine
  name: type
  type: string
- description: Report owner username
  name: owner
  type: string
- description: When the report was created
  name: createdTime
  type: string
- description: When the report was last modified
  name: modifiedTime
  type: string
- description: Parent folder system identifier
  name: folderId
  type: integer
- description: Report prompt parameters
  name: parameters
  type: array
- description: Data providers feeding the report
  name: dataProviders
  type: array
- description: ''
  name: schedule
  type: object
provider_name: SAP Business Intelligence
provider_slug: sap-bi
schema_file: json-schema/sap-bi-report-schema.json
slug: sap-bi-report
source_filename: sap-bi-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.sap.com/schemas/sap-bi/report.json\",\n  \"title\": \"SAP BusinessObjects Report\",\n  \"description\": \"A report document in SAP BusinessObjects BI Platform, representing Crystal Reports, Web Intelligence documents, or publications managed through the content management system.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Report unique system identifier (SI_ID)\"\n    },\n    \"cuid\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster unique identifier (SI_CUID)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Report name\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Report description\"\n    },\n    \"type\": {\n      \"type\"\
  : \"string\",\n      \"enum\": [\"CrystalReport\", \"Webi\", \"Publication\"],\n      \"description\": \"Report type indicating the reporting engine\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Report owner username\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the report was created\"\n    },\n    \"modifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the report was last modified\"\n    },\n    \"folderId\": {\n      \"type\": \"integer\",\n      \"description\": \"Parent folder system identifier\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Parameter\"\n      },\n      \"description\": \"Report prompt parameters\"\n    },\n    \"dataProviders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DataProvider\"\n     \
  \ },\n      \"description\": \"Data providers feeding the report\"\n    },\n    \"schedule\": {\n      \"$ref\": \"#/$defs/Schedule\"\n    }\n  },\n  \"$defs\": {\n    \"Parameter\": {\n      \"type\": \"object\",\n      \"description\": \"A prompt parameter that accepts user input when running a report\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Parameter identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Parameter display name\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Parameter data type\"\n        },\n        \"optional\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the parameter is optional\"\n        },\n        \"allowMultipleValues\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether multiple values can be provided\"\n        },\n        \"defaultValues\"\
  : {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Default parameter values\"\n        }\n      }\n    },\n    \"DataProvider\": {\n      \"type\": \"object\",\n      \"description\": \"A data source connection providing data to the report\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Data provider identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Data provider name\"\n        },\n        \"dataSourceType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of data source\"\n        },\n        \"query\": {\n          \"type\": \"string\",\n          \"description\": \"Query text\"\n        }\n      }\n    },\n    \"Schedule\": {\n      \"type\": \"object\",\n      \"description\": \"Scheduling configuration for automated report execution\",\n      \"properties\"\
  : {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Schedule unique identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Schedule name\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"Active\", \"Paused\", \"Completed\"],\n          \"description\": \"Schedule status\"\n        },\n        \"recurrenceType\": {\n          \"type\": \"string\",\n          \"enum\": [\"Once\", \"Daily\", \"Weekly\", \"Monthly\"],\n          \"description\": \"Recurrence pattern\"\n        },\n        \"nextRunTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Next scheduled run time\"\n        },\n        \"format\": {\n          \"type\": \"string\",\n          \"enum\": [\"PDF\", \"Excel\", \"CSV\", \"HTML\"],\n          \"description\": \"Output format\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-bi/refs/heads/main/json-schema/sap-bi-report-schema.json
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Reporting
- SAP
title: SAP BusinessObjects Report
---
