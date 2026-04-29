---
description: Describes a subnet.
layout: schema
name: Subnet
properties_list:
- description: ''
  name: SubnetIdentifier
  type: object
- description: ''
  name: SubnetAvailabilityZone
  type: object
- description: ''
  name: SubnetStatus
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-subnet-schema.json
slug: redshift-subnet
source_filename: redshift-subnet-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SubnetIdentifier\": {},\n    \"SubnetAvailabilityZone\": {},\n    \"SubnetStatus\": {}\n  },\n  \"description\": \"Describes a subnet.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-subnet-schema.json\",\n  \"title\": \"Subnet\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-subnet-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: Subnet
---
