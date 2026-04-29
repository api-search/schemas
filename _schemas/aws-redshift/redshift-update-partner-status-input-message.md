---
description: UpdatePartnerStatusInputMessage schema from Amazon Redshift
layout: schema
name: UpdatePartnerStatusInputMessage
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
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusMessage
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-update-partner-status-input-message-schema.json
slug: redshift-update-partner-status-input-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {},\n    \"ClusterIdentifier\": {},\n    \"DatabaseName\": {},\n    \"PartnerName\": {},\n    \"Status\": {},\n    \"StatusMessage\": {}\n  },\n  \"required\": [\n    \"AccountId\",\n    \"ClusterIdentifier\",\n    \"DatabaseName\",\n    \"PartnerName\",\n    \"Status\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-update-partner-status-input-message-schema.json\",\n  \"title\": \"UpdatePartnerStatusInputMessage\",\n  \"description\": \"UpdatePartnerStatusInputMessage schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-update-partner-status-input-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: UpdatePartnerStatusInputMessage
---
