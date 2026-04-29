---
description: Describes the status of changes to HSM settings.
layout: schema
name: HsmStatus
properties_list:
- description: ''
  name: HsmClientCertificateIdentifier
  type: object
- description: ''
  name: HsmConfigurationIdentifier
  type: object
- description: ''
  name: Status
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-hsm-status-schema.json
slug: redshift-hsm-status
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"HsmClientCertificateIdentifier\": {},\n    \"HsmConfigurationIdentifier\": {},\n    \"Status\": {}\n  },\n  \"description\": \"Describes the status of changes to HSM settings.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-hsm-status-schema.json\",\n  \"title\": \"HsmStatus\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-hsm-status-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: HsmStatus
---
