---
description: Form for creating a transient report instance
layout: schema
name: InstanceForm
properties_list:
- description: Whether to suppress data retrieval during instance creation
  name: SuppressData
  type: boolean
- description: ''
  name: ConnectionInfo
  type: object
provider_name: Crystal Reports
provider_slug: crystal-reports
schema_file: json-schema/crystal-reports-instance-form-schema.json
slug: crystal-reports-instance-form
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-instance-form-schema.json\",\n  \"title\": \"InstanceForm\",\n  \"description\": \"Form for creating a transient report instance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SuppressData\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to suppress data retrieval during instance creation\",\n      \"example\": false\n    },\n    \"ConnectionInfo\": {\n      \"$ref\": \"#/components/schemas/ConnectionInfo\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/json-schema/crystal-reports-instance-form-schema.json
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
title: InstanceForm
---
