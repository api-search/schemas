---
description: Describes a Redshift-managed VPC endpoint.
layout: schema
name: EndpointAccess
properties_list:
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: ResourceOwner
  type: object
- description: ''
  name: SubnetGroupName
  type: object
- description: ''
  name: EndpointStatus
  type: object
- description: ''
  name: EndpointName
  type: object
- description: ''
  name: EndpointCreateTime
  type: object
- description: ''
  name: Port
  type: object
- description: ''
  name: Address
  type: object
- description: ''
  name: VpcSecurityGroups
  type: object
- description: The connection endpoint for connecting to an Amazon Redshift cluster through the proxy.
  name: VpcEndpoint
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-endpoint-access-schema.json
slug: redshift-endpoint-access
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: EndpointAccess
---
