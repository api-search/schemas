---
description: CreateHsmConfigurationResult schema from Amazon Redshift
layout: schema
name: CreateHsmConfigurationResult
properties_list:
- description: Returns information about an HSM configuration, which is an object that describes to Amazon Redshift clusters the information they require to connect to an HSM where they can store database encryption
  name: HsmConfiguration
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-create-hsm-configuration-result-schema.json
slug: redshift-create-hsm-configuration-result
source_filename: redshift-create-hsm-configuration-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"HsmConfiguration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"HsmConfigurationIdentifier\": {},\n        \"Description\": {},\n        \"HsmIpAddress\": {},\n        \"HsmPartitionName\": {},\n        \"Tags\": {}\n      },\n      \"description\": \"Returns information about an HSM configuration, which is an object that describes to Amazon Redshift clusters the information they require to connect to an HSM where they can store database encryption keys.\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-hsm-configuration-result-schema.json\",\n  \"title\": \"CreateHsmConfigurationResult\",\n  \"description\": \"CreateHsmConfigurationResult schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-hsm-configuration-result-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: CreateHsmConfigurationResult
---
