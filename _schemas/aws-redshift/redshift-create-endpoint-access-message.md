---
description: CreateEndpointAccessMessage schema from Amazon Redshift
layout: schema
name: CreateEndpointAccessMessage
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: ResourceOwner
  type: object
- description: ''
  name: EndpointName
  type: object
- description: ''
  name: SubnetGroupName
  type: object
- description: ''
  name: VpcSecurityGroupIds
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-create-endpoint-access-message-schema.json
slug: redshift-create-endpoint-access-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"ResourceOwner\": {},\n    \"EndpointName\": {},\n    \"SubnetGroupName\": {},\n    \"VpcSecurityGroupIds\": {}\n  },\n  \"required\": [\n    \"EndpointName\",\n    \"SubnetGroupName\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-endpoint-access-message-schema.json\",\n  \"title\": \"CreateEndpointAccessMessage\",\n  \"description\": \"CreateEndpointAccessMessage schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-endpoint-access-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: CreateEndpointAccessMessage
---
