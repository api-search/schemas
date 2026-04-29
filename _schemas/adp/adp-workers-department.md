---
description: ''
layout: schema
name: Department
properties_list:
- description: ''
  name: departmentCode
  type: string
- description: ''
  name: departmentName
  type: string
- description: ''
  name: parentDepartmentCode
  type: string
provider_name: ADP
provider_slug: adp
schema_file: json-schema/adp-workers-department-schema.json
slug: adp-workers-department
source_filename: adp-workers-department-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Department\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"departmentCode\": {\n      \"type\": \"string\"\n    },\n    \"departmentName\": {\n      \"type\": \"string\"\n    },\n    \"parentDepartmentCode\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/json-schema/adp-workers-department-schema.json
tags:
- Benefits
- HCM
- HR
- Payroll
- Workforce
title: Department
---
