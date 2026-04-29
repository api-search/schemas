---
description: Describes a connection endpoint.
layout: schema
name: Endpoint
properties_list:
- description: ''
  name: Address
  type: object
- description: ''
  name: Port
  type: object
- description: ''
  name: VpcEndpoints
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-endpoint-schema.json
slug: redshift-endpoint
source_filename: redshift-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Address\": {},\n    \"Port\": {},\n    \"VpcEndpoints\": {}\n  },\n  \"description\": \"Describes a connection endpoint.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-endpoint-schema.json\",\n  \"title\": \"Endpoint\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-endpoint-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: Endpoint
---
