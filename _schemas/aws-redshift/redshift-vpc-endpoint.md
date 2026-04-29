---
description: The connection endpoint for connecting to an Amazon Redshift cluster through the proxy.
layout: schema
name: VpcEndpoint
properties_list:
- description: ''
  name: VpcEndpointId
  type: object
- description: ''
  name: VpcId
  type: object
- description: ''
  name: NetworkInterfaces
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-vpc-endpoint-schema.json
slug: redshift-vpc-endpoint
source_filename: redshift-vpc-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcEndpointId\": {},\n    \"VpcId\": {},\n    \"NetworkInterfaces\": {}\n  },\n  \"description\": \"The connection endpoint for connecting to an Amazon Redshift cluster through the proxy.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-vpc-endpoint-schema.json\",\n  \"title\": \"VpcEndpoint\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-vpc-endpoint-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: VpcEndpoint
---
