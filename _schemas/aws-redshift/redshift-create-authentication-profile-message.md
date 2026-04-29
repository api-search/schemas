---
description: CreateAuthenticationProfileMessage schema from Amazon Redshift
layout: schema
name: CreateAuthenticationProfileMessage
properties_list:
- description: ''
  name: AuthenticationProfileName
  type: object
- description: ''
  name: AuthenticationProfileContent
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-create-authentication-profile-message-schema.json
slug: redshift-create-authentication-profile-message
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuthenticationProfileName\": {},\n    \"AuthenticationProfileContent\": {}\n  },\n  \"required\": [\n    \"AuthenticationProfileName\",\n    \"AuthenticationProfileContent\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-authentication-profile-message-schema.json\",\n  \"title\": \"CreateAuthenticationProfileMessage\",\n  \"description\": \"CreateAuthenticationProfileMessage schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-authentication-profile-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: CreateAuthenticationProfileMessage
---
