---
description: Returns information about an HSM configuration, which is an object that describes to Amazon Redshift clusters the information they require to connect to an HSM where they can store database encryption keys.
layout: schema
name: HsmConfiguration
properties_list:
- description: ''
  name: HsmConfigurationIdentifier
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: HsmIpAddress
  type: object
- description: ''
  name: HsmPartitionName
  type: object
- description: ''
  name: Tags
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-hsm-configuration-schema.json
slug: redshift-hsm-configuration
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"HsmConfigurationIdentifier\": {},\n    \"Description\": {},\n    \"HsmIpAddress\": {},\n    \"HsmPartitionName\": {},\n    \"Tags\": {}\n  },\n  \"description\": \"Returns information about an HSM configuration, which is an object that describes to Amazon Redshift clusters the information they require to connect to an HSM where they can store database encryption keys.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-hsm-configuration-schema.json\",\n  \"title\": \"HsmConfiguration\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-hsm-configuration-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: HsmConfiguration
---
