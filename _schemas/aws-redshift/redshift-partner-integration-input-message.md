---
description: PartnerIntegrationInputMessage schema from Amazon Redshift
layout: schema
name: PartnerIntegrationInputMessage
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: ClusterIdentifier
  type: object
- description: ''
  name: DatabaseName
  type: object
- description: ''
  name: PartnerName
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-partner-integration-input-message-schema.json
slug: redshift-partner-integration-input-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {},\n    \"ClusterIdentifier\": {},\n    \"DatabaseName\": {},\n    \"PartnerName\": {}\n  },\n  \"required\": [\n    \"AccountId\",\n    \"ClusterIdentifier\",\n    \"DatabaseName\",\n    \"PartnerName\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-partner-integration-input-message-schema.json\",\n  \"title\": \"PartnerIntegrationInputMessage\",\n  \"description\": \"PartnerIntegrationInputMessage schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-partner-integration-input-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: PartnerIntegrationInputMessage
---
