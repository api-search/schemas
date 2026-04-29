---
description: Describes a network interface.
layout: schema
name: NetworkInterface
properties_list:
- description: ''
  name: NetworkInterfaceId
  type: object
- description: ''
  name: SubnetId
  type: object
- description: ''
  name: PrivateIpAddress
  type: object
- description: ''
  name: AvailabilityZone
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-network-interface-schema.json
slug: redshift-network-interface
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"NetworkInterfaceId\": {},\n    \"SubnetId\": {},\n    \"PrivateIpAddress\": {},\n    \"AvailabilityZone\": {}\n  },\n  \"description\": \"Describes a network interface. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-network-interface-schema.json\",\n  \"title\": \"NetworkInterface\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-network-interface-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: NetworkInterface
---
