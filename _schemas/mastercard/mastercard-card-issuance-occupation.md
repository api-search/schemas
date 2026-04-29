---
description: ''
layout: schema
name: Occupation
properties_list:
- description: Employer Name. <BR/>This field is required if configured as **Business Mandatory**<font color='red'>* </font>.
  name: employerName
  type: string
- description: Department of client. <BR/>This field is required if configured as **Business Mandatory**<font color='red'>* </font>.
  name: department
  type: string
- description: Employee ID of client. <BR/>This field is required if configured as **Business Mandatory**<font color='red'>* </font>.
  name: employeeId
  type: string
- description: Joining date of current job. <BR/>This field is required if configured as **Business Mandatory**<font color='red'>* </font>. <br/> Format - It is expressed in ISO 8601 - `YYYY-MM-DD`
  name: joiningDate
  type: string
- description: Duration (in years) of employment with current employer. <BR/>This field is required if configured as **Business Mandatory**<font color='red'>* </font>.
  name: employmentDuration
  type: integer
- description: Annual income of client. <BR/>This field is required if configured as **Business Mandatory**<font color='red'>* </font>.
  name: netAnnualIncome
  type: integer
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-occupation-schema.json
slug: mastercard-card-issuance-occupation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Occupation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"employerName\": {\n      \"type\": \"string\",\n      \"description\": \"Employer Name. <BR/>This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"Department of client. <BR/>This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"employeeId\": {\n      \"type\": \"string\",\n      \"description\": \"Employee ID of client. <BR/>This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"joiningDate\": {\n      \"type\": \"string\",\n      \"description\": \"Joining date of current job. <BR/>This field is required if configured as **Business Mandatory**<font color='red'>* </font>. <br/> Format - It is expressed\
  \ in ISO 8601 - `YYYY-MM-DD`\"\n    },\n    \"employmentDuration\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration (in years) of employment with current employer. <BR/>This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    },\n    \"netAnnualIncome\": {\n      \"type\": \"integer\",\n      \"description\": \"Annual income of client. <BR/>This field is required if configured as **Business Mandatory**<font color='red'>* </font>.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-occupation-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Occupation
---
