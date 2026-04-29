---
description: Describes the status of the elastic IP (EIP) address.
layout: schema
name: ElasticIpStatus
properties_list:
- description: ''
  name: ElasticIp
  type: object
- description: ''
  name: Status
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-elastic-ip-status-schema.json
slug: redshift-elastic-ip-status
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ElasticIp\": {},\n    \"Status\": {}\n  },\n  \"description\": \"Describes the status of the elastic IP (EIP) address.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-elastic-ip-status-schema.json\",\n  \"title\": \"ElasticIpStatus\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-elastic-ip-status-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ElasticIpStatus
---
