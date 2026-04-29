---
description: Contact creation request
layout: schema
name: ContactCreate
properties_list:
- description: Contact full name
  name: name
  type: string
- description: Contact first name
  name: first_name
  type: string
- description: Contact middle name
  name: middle_name
  type: string
- description: Contact last name
  name: last_name
  type: string
- description: Contact user ID
  name: user_name
  type: string
- description: Contact email address
  name: email
  type: string
- description: Contact business phone number
  name: phone
  type: string
- description: Contact mobile phone number
  name: mobile_phone
  type: string
- description: Contact home phone number
  name: home_phone
  type: string
- description: Contact business title
  name: title
  type: string
- description: Contact employee number
  name: employee_number
  type: string
- description: Sys_id of the company record
  name: company
  type: string
- description: Sys_id of the account record
  name: account
  type: string
- description: Sys_id of the department
  name: department
  type: string
- description: Sys_id of the direct supervisor
  name: manager
  type: string
- description: Sys_id of the location
  name: location
  type: string
- description: Sys_id of the building
  name: building
  type: string
- description: Contact street address
  name: street
  type: string
- description: City in which the contact resides
  name: city
  type: string
- description: State in which the contact resides
  name: state
  type: string
- description: Contact zip code
  name: zip
  type: string
- description: Country code
  name: country
  type: string
- description: Flag indicating whether the contact is active
  name: active
  type: boolean
- description: Flag indicating whether the contact has VIP status
  name: vip
  type: boolean
- description: Flag indicating if the contact is locked-out
  name: locked_out
  type: boolean
- description: Flag indicating whether the contact can only access services through the web
  name: web_service_access_only
  type: boolean
- description: Flag indicating whether the contact is an internal integration user
  name: internal_integration_user
  type: boolean
- description: Flag indicating whether multifactor authorization is required
  name: enable_multifactor_authn
  type: boolean
- description: Flag indicating whether the contact location is obtained through geotracking
  name: geolocation_tracked
  type: boolean
- description: Indicates whether the contact should receive notifications (1=Disabled, 2=Enabled)
  name: notification
  type: integer
- description: Calendar application that the contact uses (1=Outlook)
  name: calendar_integration
  type: integer
- description: Number of failed login attempts
  name: failed_attempts
  type: integer
- description: Latitude coordinate of the contact
  name: latitude
  type: number
- description: Longitude coordinate of the contact
  name: longitude
  type: number
- description: Time zone in which the contact resides
  name: time_zone
  type: string
- description: Format in which to display dates
  name: date_format
  type: string
- description: Format in which to display time
  name: time_format
  type: string
- description: Country code of the contact primary language
  name: preferred_language
  type: string
- description: Contact gender
  name: gender
  type: string
- description: Photo image of the contact
  name: photo
  type: string
- description: Introduction
  name: introduction
  type: string
- description: Source of the contact
  name: source
  type: string
- description: List of user roles associated with the contact
  name: roles
  type: string
- description: Sys_id of the cost center
  name: cost_center
  type: string
- description: Sys_id of the work schedule
  name: schedule
  type: string
- description: Sys_id of the time sheet policy
  name: time_sheet_policy
  type: string
- description: Sys_id of the default perspective
  name: default_perspective
  type: string
- description: Sys_id of the LDAP server
  name: ldap_server
  type: string
- description: Status of the agent
  name: agent_status
  type: string
- description: Indicates the timeliness of dispatched service personnel
  name: on_schedule
  type: string
- description: Education status of the contact
  name: edu_status
  type: string
- description: Date and time the contact logged in to the system
  name: last_login_time
  type: string
- description: Device the consumer used the last time they logged in
  name: last_login_device
  type: string
- description: Social media channel (Twitter, Facebook, Instagram, etc.)
  name: social_channel
  type: string
- description: User handle on the social media channel
  name: social_handle
  type: string
- description: URL to the contact's social channel profile
  name: social_handle_url
  type: string
provider_name: ServiceNow
provider_slug: servicenow
schema_file: json-schema/contact-contact-create-schema.json
slug: contact-contact-create
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Contact creation request\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Contact full name\",\n      \"example\": \"Example Title\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"Contact first name\",\n      \"example\": \"example_value\"\n    },\n    \"middle_name\": {\n      \"type\": \"string\",\n      \"description\": \"Contact middle name\",\n      \"example\": \"example_value\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Contact last name\",\n      \"example\": \"example_value\"\n    },\n    \"user_name\": {\n      \"type\": \"string\",\n      \"description\": \"Contact user ID\",\n      \"example\": \"example_value\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Contact email address\",\n      \"example\": \"user@example.com\"\n    },\n    \"phone\": {\n    \
  \  \"type\": \"string\",\n      \"description\": \"Contact business phone number\",\n      \"example\": \"example_value\"\n    },\n    \"mobile_phone\": {\n      \"type\": \"string\",\n      \"description\": \"Contact mobile phone number\",\n      \"example\": \"example_value\"\n    },\n    \"home_phone\": {\n      \"type\": \"string\",\n      \"description\": \"Contact home phone number\",\n      \"example\": \"example_value\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Contact business title\",\n      \"example\": \"Example Title\"\n    },\n    \"employee_number\": {\n      \"type\": \"string\",\n      \"description\": \"Contact employee number\",\n      \"example\": \"example_value\"\n    },\n    \"company\": {\n      \"type\": \"string\",\n      \"description\": \"Sys_id of the company record\",\n      \"example\": \"example_value\"\n    },\n    \"account\": {\n      \"type\": \"string\",\n      \"description\": \"Sys_id of the account record\"\
  ,\n      \"example\": 42\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"Sys_id of the department\",\n      \"example\": \"example_value\"\n    },\n    \"manager\": {\n      \"type\": \"string\",\n      \"description\": \"Sys_id of the direct supervisor\",\n      \"example\": \"example_value\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Sys_id of the location\",\n      \"example\": \"example_value\"\n    },\n    \"building\": {\n      \"type\": \"string\",\n      \"description\": \"Sys_id of the building\",\n      \"example\": \"example_value\"\n    },\n    \"street\": {\n      \"type\": \"string\",\n      \"description\": \"Contact street address\",\n      \"example\": \"example_value\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City in which the contact resides\",\n      \"example\": \"example_value\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"State in which the contact resides\",\n      \"example\": \"example_value\"\n    },\n    \"zip\": {\n      \"type\": \"string\",\n      \"description\": \"Contact zip code\",\n      \"example\": \"example_value\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country code\",\n      \"example\": 42\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating whether the contact is active\",\n      \"example\": true\n    },\n    \"vip\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating whether the contact has VIP status\",\n      \"example\": true\n    },\n    \"locked_out\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating if the contact is locked-out\",\n      \"example\": true\n    },\n    \"web_service_access_only\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating whether the contact can only access services through the web\",\n   \
  \   \"example\": true\n    },\n    \"internal_integration_user\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating whether the contact is an internal integration user\",\n      \"example\": true\n    },\n    \"enable_multifactor_authn\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating whether multifactor authorization is required\",\n      \"example\": true\n    },\n    \"geolocation_tracked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Flag indicating whether the contact location is obtained through geotracking\",\n      \"example\": true\n    },\n    \"notification\": {\n      \"type\": \"integer\",\n      \"description\": \"Indicates whether the contact should receive notifications (1=Disabled, 2=Enabled)\",\n      \"example\": 1,\n      \"enum\": [\n        1,\n        2\n      ]\n    },\n    \"calendar_integration\": {\n      \"type\": \"integer\",\n      \"description\": \"Calendar application that the contact uses\
  \ (1=Outlook)\",\n      \"example\": 10\n    },\n    \"failed_attempts\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of failed login attempts\",\n      \"example\": 10\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"description\": \"Latitude coordinate of the contact\",\n      \"format\": \"float\",\n      \"example\": 42.5\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"description\": \"Longitude coordinate of the contact\",\n      \"format\": \"float\",\n      \"example\": 42.5\n    },\n    \"time_zone\": {\n      \"type\": \"string\",\n      \"description\": \"Time zone in which the contact resides\",\n      \"example\": \"example_value\"\n    },\n    \"date_format\": {\n      \"type\": \"string\",\n      \"description\": \"Format in which to display dates\",\n      \"example\": \"dd/mm/yyyy\",\n      \"enum\": [\n        \"dd/mm/yyyy\",\n        \"dd-mm-yyyy\",\n        \"dd.mm.yyyy\",\n        \"mm-dd-yyyy\",\n        \"\
  yyyy-mm-dd\"\n      ]\n    },\n    \"time_format\": {\n      \"type\": \"string\",\n      \"description\": \"Format in which to display time\",\n      \"example\": \"hh.mm.ss a\",\n      \"enum\": [\n        \"hh.mm.ss a\",\n        \"hh:mm:ss a\",\n        \"HH.mm.ss\",\n        \"HH:mm:ss\"\n      ]\n    },\n    \"preferred_language\": {\n      \"type\": \"string\",\n      \"description\": \"Country code of the contact primary language\",\n      \"example\": \"example_value\"\n    },\n    \"gender\": {\n      \"type\": \"string\",\n      \"description\": \"Contact gender\",\n      \"example\": \"example_value\"\n    },\n    \"photo\": {\n      \"type\": \"string\",\n      \"description\": \"Photo image of the contact\",\n      \"example\": \"example_value\"\n    },\n    \"introduction\": {\n      \"type\": \"string\",\n      \"description\": \"Introduction\",\n      \"example\": \"example_value\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source\
  \ of the contact\",\n      \"example\": \"example_value\"\n    },\n    \"roles\": {\n      \"type\": \"string\",\n      \"description\": \"List of user roles associated with the contact\",\n      \"example\": \"example_value\"\n    },\n    \"cost_center\": {\n      \"type\": \"string\",\n      \"description\": \"Sys_id of the cost center\",\n      \"example\": \"example_value\"\n    },\n    \"schedule\": {\n      \"type\": \"string\",\n      \"description\": \"Sys_id of the work schedule\",\n      \"example\": \"example_value\"\n    },\n    \"time_sheet_policy\": {\n      \"type\": \"string\",\n      \"description\": \"Sys_id of the time sheet policy\",\n      \"example\": \"example_value\"\n    },\n    \"default_perspective\": {\n      \"type\": \"string\",\n      \"description\": \"Sys_id of the default perspective\",\n      \"example\": \"example_value\"\n    },\n    \"ldap_server\": {\n      \"type\": \"string\",\n      \"description\": \"Sys_id of the LDAP server\",\n      \"example\"\
  : \"example_value\"\n    },\n    \"agent_status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the agent\",\n      \"example\": \"Off work\",\n      \"enum\": [\n        \"Off work\",\n        \"On break\",\n        \"On route\",\n        \"On site\"\n      ]\n    },\n    \"on_schedule\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates the timeliness of dispatched service personnel\",\n      \"example\": \"Ahead\",\n      \"enum\": [\n        \"Ahead\",\n        \"behind_less30\",\n        \"behind_30to60\",\n        \"behind_more60\",\n        \"on_time\"\n      ]\n    },\n    \"edu_status\": {\n      \"type\": \"string\",\n      \"description\": \"Education status of the contact\",\n      \"example\": \"example_value\"\n    },\n    \"last_login_time\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time the contact logged in to the system\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n  \
  \  },\n    \"last_login_device\": {\n      \"type\": \"string\",\n      \"description\": \"Device the consumer used the last time they logged in\",\n      \"example\": \"example_value\"\n    },\n    \"social_channel\": {\n      \"type\": \"string\",\n      \"description\": \"Social media channel (Twitter, Facebook, Instagram, etc.)\",\n      \"example\": \"example_value\"\n    },\n    \"social_handle\": {\n      \"type\": \"string\",\n      \"description\": \"User handle on the social media channel\",\n      \"example\": \"example_value\"\n    },\n    \"social_handle_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to the contact's social channel profile\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContactCreate\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/json-schema/contact-contact-create-schema.json
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
title: ContactCreate
---
