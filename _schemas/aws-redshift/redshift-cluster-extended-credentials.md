---
description: ClusterExtendedCredentials schema from Amazon Redshift
layout: schema
name: ClusterExtendedCredentials
properties_list:
- description: ''
  name: DbUser
  type: object
- description: ''
  name: DbPassword
  type: object
- description: ''
  name: Expiration
  type: object
- description: ''
  name: NextRefreshTime
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-cluster-extended-credentials-schema.json
slug: redshift-cluster-extended-credentials
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DbUser\": {},\n    \"DbPassword\": {},\n    \"Expiration\": {},\n    \"NextRefreshTime\": {}\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-extended-credentials-schema.json\",\n  \"title\": \"ClusterExtendedCredentials\",\n  \"description\": \"ClusterExtendedCredentials schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-cluster-extended-credentials-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ClusterExtendedCredentials
---
