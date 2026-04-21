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
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: EndpointAuthorization
---
