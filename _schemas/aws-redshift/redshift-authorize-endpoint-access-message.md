---
description: AuthorizeEndpointAccessMessage schema from Amazon Redshift
layout: schema
name: AuthorizeEndpointAccessMessage
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: Account
  type: object
- description: ''
  name: VpcIds
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-authorize-endpoint-access-message-schema.json
slug: redshift-authorize-endpoint-access-message
source_filename: redshift-authorize-endpoint-access-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"Account\": {},\n    \"VpcIds\": {}\n  },\n  \"required\": [\n    \"Account\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-authorize-endpoint-access-message-schema.json\",\n  \"title\": \"AuthorizeEndpointAccessMessage\",\n  \"description\": \"AuthorizeEndpointAccessMessage schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-authorize-endpoint-access-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: AuthorizeEndpointAccessMessage
---
