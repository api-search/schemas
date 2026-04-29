---
description: <p/>
layout: schema
name: CreateHsmConfigurationMessage
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
  name: HsmPartitionPassword
  type: object
- description: ''
  name: HsmServerPublicCertificate
  type: object
- description: ''
  name: Tags
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-create-hsm-configuration-message-schema.json
slug: redshift-create-hsm-configuration-message
source_filename: redshift-create-hsm-configuration-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"HsmConfigurationIdentifier\": {},\n    \"Description\": {},\n    \"HsmIpAddress\": {},\n    \"HsmPartitionName\": {},\n    \"HsmPartitionPassword\": {},\n    \"HsmServerPublicCertificate\": {},\n    \"Tags\": {}\n  },\n  \"required\": [\n    \"HsmConfigurationIdentifier\",\n    \"Description\",\n    \"HsmIpAddress\",\n    \"HsmPartitionName\",\n    \"HsmPartitionPassword\",\n    \"HsmServerPublicCertificate\"\n  ],\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-hsm-configuration-message-schema.json\",\n  \"title\": \"CreateHsmConfigurationMessage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-create-hsm-configuration-message-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: CreateHsmConfigurationMessage
---
