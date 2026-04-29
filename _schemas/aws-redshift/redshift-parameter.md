---
description: Describes a parameter in a cluster parameter group.
layout: schema
name: Parameter
properties_list:
- description: ''
  name: ParameterName
  type: object
- description: ''
  name: ParameterValue
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Source
  type: object
- description: ''
  name: DataType
  type: object
- description: ''
  name: AllowedValues
  type: object
- description: ''
  name: ApplyType
  type: object
- description: ''
  name: IsModifiable
  type: object
- description: ''
  name: MinimumEngineVersion
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-parameter-schema.json
slug: redshift-parameter
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ParameterName\": {},\n    \"ParameterValue\": {},\n    \"Description\": {},\n    \"Source\": {},\n    \"DataType\": {},\n    \"AllowedValues\": {},\n    \"ApplyType\": {},\n    \"IsModifiable\": {},\n    \"MinimumEngineVersion\": {}\n  },\n  \"description\": \"Describes a parameter in a cluster parameter group.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-parameter-schema.json\",\n  \"title\": \"Parameter\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-parameter-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: Parameter
---
