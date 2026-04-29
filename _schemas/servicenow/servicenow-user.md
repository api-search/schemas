---
description: A ServiceNow user record from the sys_user table representing a person who can authenticate and interact with the platform.
layout: schema
name: ServiceNow User
properties_list:
- description: The unique 32-character system identifier for the user.
  name: sys_id
  type: string
- description: The login user name.
  name: user_name
  type: string
- description: The user's first name.
  name: first_name
  type:
  - string
  - 'null'
- description: The user's middle name.
  name: middle_name
  type:
  - string
  - 'null'
- description: The user's last name.
  name: last_name
  type:
  - string
  - 'null'
- description: The user's full display name.
  name: name
  type:
  - string
  - 'null'
- description: The user's email address.
  name: email
  type:
  - string
  - 'null'
- description: The user's business phone number.
  name: phone
  type:
  - string
  - 'null'
- description: The user's mobile phone number.
  name: mobile_phone
  type:
  - string
  - 'null'
- description: The user's job title.
  name: title
  type:
  - string
  - 'null'
- description: The employee number.
  name: employee_number
  type:
  - string
  - 'null'
- description: The user's department.
  name: department
  type: object
- description: The user's company.
  name: company
  type: object
- description: The user's direct manager.
  name: manager
  type: object
- description: The user's primary location.
  name: location
  type: object
- description: The user's building.
  name: building
  type: object
- description: The user's cost center.
  name: cost_center
  type: object
- description: The user's time zone.
  name: time_zone
  type:
  - string
  - 'null'
- description: Whether the user account is active.
  name: active
  type: boolean
- description: Whether the user account is locked out.
  name: locked_out
  type: boolean
- description: Whether the user has VIP status.
  name: vip
  type: boolean
- description: Comma-separated list of role names assigned to the user.
  name: roles
  type:
  - string
  - 'null'
- description: The source from which the user record was created.
  name: source
  type:
  - string
  - 'null'
- description: The date and time of the user's last login.
  name: last_login_time
  type:
  - string
  - 'null'
- description: The number of failed login attempts.
  name: failed_attempts
  type:
  - integer
  - 'null'
- description: The URL or reference to the user's photo.
  name: photo
  type:
  - string
  - 'null'
- description: The date and time the record was created.
  name: sys_created_on
  type: string
- description: The user who created the record.
  name: sys_created_by
  type: string
- description: The date and time the record was last updated.
  name: sys_updated_on
  type: string
- description: The user who last updated the record.
  name: sys_updated_by
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/servicenow-user-schema.json
slug: servicenow-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://servicenow.com/schemas/servicenow/user.json\",\n  \"title\": \"ServiceNow User\",\n  \"description\": \"A ServiceNow user record from the sys_user table representing a person who can authenticate and interact with the platform.\",\n  \"type\": \"object\",\n  \"required\": [\"sys_id\", \"user_name\"],\n  \"properties\": {\n    \"sys_id\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[a-f0-9]{32}$\",\n      \"description\": \"The unique 32-character system identifier for the user.\"\n    },\n    \"user_name\": {\n      \"type\": \"string\",\n      \"maxLength\": 40,\n      \"description\": \"The login user name.\"\n    },\n    \"first_name\": {\n      \"type\": [\"string\", \"null\"],\n      \"maxLength\": 50,\n      \"description\": \"The user's first name.\"\n    },\n    \"middle_name\": {\n      \"type\": [\"string\", \"null\"],\n      \"maxLength\": 50,\n      \"description\"\
  : \"The user's middle name.\"\n    },\n    \"last_name\": {\n      \"type\": [\"string\", \"null\"],\n      \"maxLength\": 50,\n      \"description\": \"The user's last name.\"\n    },\n    \"name\": {\n      \"type\": [\"string\", \"null\"],\n      \"maxLength\": 151,\n      \"description\": \"The user's full display name.\"\n    },\n    \"email\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"email\",\n      \"description\": \"The user's email address.\"\n    },\n    \"phone\": {\n      \"type\": [\"string\", \"null\"],\n      \"maxLength\": 40,\n      \"description\": \"The user's business phone number.\"\n    },\n    \"mobile_phone\": {\n      \"type\": [\"string\", \"null\"],\n      \"maxLength\": 40,\n      \"description\": \"The user's mobile phone number.\"\n    },\n    \"title\": {\n      \"type\": [\"string\", \"null\"],\n      \"maxLength\": 60,\n      \"description\": \"The user's job title.\"\n    },\n    \"employee_number\": {\n      \"type\": [\"string\"\
  , \"null\"],\n      \"description\": \"The employee number.\"\n    },\n    \"department\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The user's department.\"\n    },\n    \"company\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The user's company.\"\n    },\n    \"manager\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The user's direct manager.\"\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The user's primary location.\"\n    },\n    \"building\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The user's building.\"\n    },\n    \"cost_center\": {\n      \"$ref\": \"#/$defs/ReferenceField\",\n      \"description\": \"The user's cost center.\"\n    },\n    \"time_zone\": {\n      \"type\": [\"string\", \"null\"],\n      \"maxLength\": 40,\n      \"description\": \"The user's time zone.\"\n    },\n    \"active\": {\n   \
  \   \"type\": \"boolean\",\n      \"description\": \"Whether the user account is active.\"\n    },\n    \"locked_out\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user account is locked out.\"\n    },\n    \"vip\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has VIP status.\"\n    },\n    \"roles\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Comma-separated list of role names assigned to the user.\"\n    },\n    \"source\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The source from which the user record was created.\"\n    },\n    \"last_login_time\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time of the user's last login.\"\n    },\n    \"failed_attempts\": {\n      \"type\": [\"integer\", \"null\"],\n      \"minimum\": 0,\n      \"description\": \"The number of failed login attempts.\"\n    },\n    \"photo\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The URL or reference to the user's photo.\"\n    },\n    \"sys_created_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the record was created.\"\n    },\n    \"sys_created_by\": {\n      \"type\": \"string\",\n      \"description\": \"The user who created the record.\"\n    },\n    \"sys_updated_on\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the record was last updated.\"\n    },\n    \"sys_updated_by\": {\n      \"type\": \"string\",\n      \"description\": \"The user who last updated the record.\"\n    }\n  },\n  \"$defs\": {\n    \"ReferenceField\": {\n      \"type\": [\"object\", \"string\", \"null\"],\n      \"description\": \"A ServiceNow reference field that can be a sys_id string or an object containing a link and value.\",\n      \"properties\": {\n        \"link\": {\n    \
  \      \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The API URL to the referenced record.\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The sys_id of the referenced record.\"\n        },\n        \"display_value\": {\n          \"type\": \"string\",\n          \"description\": \"The display value of the referenced record.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/servicenow-user-schema.json
tags:
- Automation
- Cloud Services
- Digital Workflows
- Enterprise Platform
- IT Service Management
- ITSM
- Processes
- T1
- Workflow Automation
- Workflows
title: ServiceNow User
---
