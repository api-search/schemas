---
description: Describes an endpoint authorization for authorizing Redshift-managed VPC endpoint access to a cluster across Amazon Web Services accounts.
layout: schema
name: EndpointAuthorization
properties_list:
- description: ''
  name: Grantor
  type: object
- description: ''
  name: Grantee
  type: object
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: AuthorizeTime
  type: object
- description: ''
  name: ClusterStatus
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: AllowedAllVPCs
  type: object
- description: ''
  name: AllowedVPCs
  type: object
- description: ''
  name: EndpointCount
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-endpoint-authorization-schema.json
slug: redshift-endpoint-authorization
source_filename: redshift-endpoint-authorization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Grantor\": {},\n    \"Grantee\": {},\n    \"ClusterIdentifier\": {},\n    \"AuthorizeTime\": {},\n    \"ClusterStatus\": {},\n    \"Status\": {},\n    \"AllowedAllVPCs\": {},\n    \"AllowedVPCs\": {},\n    \"EndpointCount\": {}\n  },\n  \"description\": \"Describes an endpoint authorization for authorizing Redshift-managed VPC endpoint access to a cluster across Amazon Web Services accounts.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-endpoint-authorization-schema.json\",\n  \"title\": \"EndpointAuthorization\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-endpoint-authorization-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: EndpointAuthorization
---
