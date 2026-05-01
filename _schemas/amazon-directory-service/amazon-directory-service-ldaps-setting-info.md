---
description: Contains general information about the LDAPS settings.
layout: schema
name: LDAPSSettingInfo
properties_list:
- description: ''
  name: LDAPSStatus
  type: object
- description: ''
  name: LDAPSStatusReason
  type: object
- description: ''
  name: LastUpdatedDateTime
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-ldaps-setting-info-schema.json
slug: amazon-directory-service-ldaps-setting-info
source_filename: amazon-directory-service-ldaps-setting-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-ldaps-setting-info-schema.json\",\n  \"title\": \"LDAPSSettingInfo\",\n  \"description\": \"Contains general information about the LDAPS settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LDAPSStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LDAPSStatus\"\n        },\n        {\n          \"description\": \"The state of the LDAPS settings.\"\n        }\n      ]\n    },\n    \"LDAPSStatusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LDAPSStatusReason\"\n        },\n        {\n          \"description\": \"Describes a state change for LDAPS.\"\n        }\n      ]\n    },\n    \"LastUpdatedDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedDateTime\"\
  \n        },\n        {\n          \"description\": \"The date and time when the LDAPS settings were last updated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-ldaps-setting-info-schema.json
tags:
- Active Directory
- Authentication
- Directory Services
- Identity Management
title: LDAPSSettingInfo
---
