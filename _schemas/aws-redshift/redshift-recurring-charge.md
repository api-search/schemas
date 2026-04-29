---
description: Describes a recurring charge.
layout: schema
name: RecurringCharge
properties_list:
- description: ''
  name: RecurringChargeAmount
  type: object
- description: ''
  name: RecurringChargeFrequency
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-recurring-charge-schema.json
slug: redshift-recurring-charge
source_filename: redshift-recurring-charge-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecurringChargeAmount\": {},\n    \"RecurringChargeFrequency\": {}\n  },\n  \"description\": \"Describes a recurring charge.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-recurring-charge-schema.json\",\n  \"title\": \"RecurringCharge\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-recurring-charge-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: RecurringCharge
---
