---
description: Represents an employee record from a connected HRIS integration in the Merge Unified API.
layout: schema
name: Employee
properties_list:
- description: The unique Merge-generated identifier.
  name: id
  type: string
- description: The third-party ID of this employee.
  name: remote_id
  type: string
- description: The employee's number in the organization.
  name: employee_number
  type: string
- description: The employee's first name.
  name: first_name
  type: string
- description: The employee's last name.
  name: last_name
  type: string
- description: The employee's full display name.
  name: display_full_name
  type: string
- description: The employee's work email address.
  name: work_email
  type: string
- description: The employee's personal email address.
  name: personal_email
  type: string
- description: The employee's mobile phone number.
  name: mobile_phone_number
  type: string
- description: The employee's date of birth.
  name: date_of_birth
  type: string
- description: The date the employee started working.
  name: start_date
  type: string
- description: The date the employee was terminated.
  name: termination_date
  type: string
- description: The current employment status.
  name: employment_status
  type: string
- description: The Merge ID of this employee's manager.
  name: manager
  type: string
- description: The Merge ID of the employee's company.
  name: company
  type: string
- description: The Merge ID of the employee's team.
  name: team
  type: string
- description: The Merge ID of the employee's pay group.
  name: pay_group
  type: string
- description: Groups this employee belongs to.
  name: groups
  type: array
- description: Whether the record was deleted in the third-party platform.
  name: remote_was_deleted
  type: boolean
- description: When the Merge record was created.
  name: created_at
  type: string
- description: When the Merge record was last modified.
  name: modified_at
  type: string
provider_name: Merge
provider_slug: merge
schema_file: json-schema/hris-api-employee-schema.json
slug: hris-api-employee
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/json-schema/hris-api-employee-schema.json\",\n  \"title\": \"Employee\",\n  \"description\": \"Represents an employee record from a connected HRIS integration in the Merge Unified API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique Merge-generated identifier.\"\n    },\n    \"remote_id\": {\n      \"type\": \"string\",\n      \"description\": \"The third-party ID of this employee.\"\n    },\n    \"employee_number\": {\n      \"type\": \"string\",\n      \"description\": \"The employee's number in the organization.\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"The employee's first name.\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The employee's last name.\"\n    },\n    \"display_full_name\": {\n      \"type\": \"string\",\n      \"description\": \"The employee's full display name.\"\n    },\n    \"work_email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The employee's work email address.\"\n    },\n    \"personal_email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The employee's personal email address.\"\n    },\n    \"mobile_phone_number\": {\n      \"type\": \"string\",\n      \"description\": \"The employee's mobile phone number.\"\n    },\n    \"date_of_birth\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The employee's date of birth.\"\n    },\n    \"start_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date the employee started working.\"\n    },\n    \"termination_date\": {\n      \"type\": \"string\",\n      \"format\":\
  \ \"date-time\",\n      \"description\": \"The date the employee was terminated.\"\n    },\n    \"employment_status\": {\n      \"type\": \"string\",\n      \"enum\": [\"ACTIVE\", \"PENDING\", \"INACTIVE\"],\n      \"description\": \"The current employment status.\"\n    },\n    \"manager\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The Merge ID of this employee's manager.\"\n    },\n    \"company\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The Merge ID of the employee's company.\"\n    },\n    \"team\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The Merge ID of the employee's team.\"\n    },\n    \"pay_group\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The Merge ID of the employee's pay group.\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"\
  format\": \"uuid\"\n      },\n      \"description\": \"Groups this employee belongs to.\"\n    },\n    \"remote_was_deleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the record was deleted in the third-party platform.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the Merge record was created.\"\n    },\n    \"modified_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the Merge record was last modified.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/json-schema/hris-api-employee-schema.json
tags:
- Integrations
- Platform
- Unified API
title: Employee
---
