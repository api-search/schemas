---
description: EndpointAccesses schema from Amazon Redshift
layout: schema
name: EndpointAccesses
properties_list: []
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-endpoint-accesses-schema.json
slug: redshift-endpoint-accesses
source_filename: redshift-endpoint-accesses-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"ClusterIdentifier\": {},\n      \"ResourceOwner\": {},\n      \"SubnetGroupName\": {},\n      \"EndpointStatus\": {},\n      \"EndpointName\": {},\n      \"EndpointCreateTime\": {},\n      \"Port\": {},\n      \"Address\": {},\n      \"VpcSecurityGroups\": {},\n      \"VpcEndpoint\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"VpcEndpointId\": {\n            \"allOf\": [\n              {\n                \"$ref\": \"#/components/schemas/String\"\n              },\n              {\n                \"description\": \"The connection endpoint ID for connecting an Amazon Redshift cluster through the proxy.\"\n              }\n            ]\n          },\n          \"VpcId\": {\n            \"allOf\": [\n              {\n                \"$ref\": \"#/components/schemas/String\"\n              },\n              {\n                \"description\": \"The\
  \ VPC identifier that the endpoint is associated. \"\n              }\n            ]\n          },\n          \"NetworkInterfaces\": {\n            \"allOf\": [\n              {\n                \"$ref\": \"#/components/schemas/NetworkInterfaceList\"\n              },\n              {\n                \"description\": \"One or more network interfaces of the endpoint. Also known as an interface endpoint. \"\n              }\n            ]\n          }\n        },\n        \"description\": \"The connection endpoint for connecting to an Amazon Redshift cluster through the proxy.\"\n      }\n    },\n    \"description\": \"Describes a Redshift-managed VPC endpoint.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-endpoint-accesses-schema.json\",\n  \"title\": \"EndpointAccesses\",\n  \"description\": \"EndpointAccesses schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-endpoint-accesses-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: EndpointAccesses
---
