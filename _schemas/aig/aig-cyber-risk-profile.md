---
description: Cyber risk profile for cyber insurance underwriting
layout: schema
name: CyberRiskProfile
properties_list:
- description: Organization name
  name: organization_name
  type: string
- description: Annual revenue in USD
  name: annual_revenue
  type: number
- description: Number of employees
  name: employee_count
  type: integer
- description: Number of personal data records held
  name: data_records_count
  type: integer
- description: Multi-factor authentication enabled
  name: mfa_enabled
  type: boolean
- description: Endpoint protection solution deployed
  name: endpoint_protection
  type: boolean
- description: Data backup frequency
  name: backup_frequency
  type: string
- description: Incident response plan in place
  name: incident_response_plan
  type: boolean
- description: Number of prior data breaches
  name: prior_breaches
  type: integer
provider_name: AIG
provider_slug: aig
schema_file: json-schema/aig-cyber-risk-profile-schema.json
slug: aig-cyber-risk-profile
source_filename: aig-cyber-risk-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aig/refs/heads/main/json-schema/aig-cyber-risk-profile-schema.json\",\n  \"title\": \"CyberRiskProfile\",\n  \"description\": \"Cyber risk profile for cyber insurance underwriting\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"organization_name\": {\n      \"type\": \"string\",\n      \"description\": \"Organization name\",\n      \"example\": \"TechCorp Inc\"\n    },\n    \"annual_revenue\": {\n      \"type\": \"number\",\n      \"description\": \"Annual revenue in USD\",\n      \"example\": 10000000.0\n    },\n    \"employee_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of employees\",\n      \"example\": 200\n    },\n    \"data_records_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of personal data records held\",\n      \"example\": 100000\n    },\n    \"mfa_enabled\": {\n     \
  \ \"type\": \"boolean\",\n      \"description\": \"Multi-factor authentication enabled\",\n      \"example\": true\n    },\n    \"endpoint_protection\": {\n      \"type\": \"boolean\",\n      \"description\": \"Endpoint protection solution deployed\",\n      \"example\": true\n    },\n    \"backup_frequency\": {\n      \"type\": \"string\",\n      \"description\": \"Data backup frequency\",\n      \"example\": \"Daily\"\n    },\n    \"incident_response_plan\": {\n      \"type\": \"boolean\",\n      \"description\": \"Incident response plan in place\",\n      \"example\": true\n    },\n    \"prior_breaches\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of prior data breaches\",\n      \"example\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aig/refs/heads/main/json-schema/aig-cyber-risk-profile-schema.json
tags:
- Insurance
- Financial Services
- Property Casualty
- Cyber Insurance
- Enterprise
title: CyberRiskProfile
---
