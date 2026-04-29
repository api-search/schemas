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
source_filename: redshift-endpoint-access-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterIdentifier\": {},\n    \"ResourceOwner\": {},\n    \"SubnetGroupName\": {},\n    \"EndpointStatus\": {},\n    \"EndpointName\": {},\n    \"EndpointCreateTime\": {},\n    \"Port\": {},\n    \"Address\": {},\n    \"VpcSecurityGroups\": {},\n    \"VpcEndpoint\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"VpcEndpointId\": {},\n        \"VpcId\": {},\n        \"NetworkInterfaces\": {}\n      },\n      \"description\": \"The connection endpoint for connecting to an Amazon Redshift cluster through the proxy.\"\n    }\n  },\n  \"description\": \"Describes a Redshift-managed VPC endpoint.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-endpoint-access-schema.json\",\n  \"title\": \"EndpointAccess\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-endpoint-access-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: EndpointAccess
---
