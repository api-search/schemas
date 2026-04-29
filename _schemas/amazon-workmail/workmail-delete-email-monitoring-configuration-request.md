---
description: DeleteEmailMonitoringConfigurationRequest schema from Amazon WorkMail API
layout: schema
name: DeleteEmailMonitoringConfigurationRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-delete-email-monitoring-configuration-request-schema.json
slug: workmail-delete-email-monitoring-configuration-request
source_filename: workmail-delete-email-monitoring-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\"\n  ],\n  \"title\": \"DeleteEmailMonitoringConfigurationRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The ID of the organization from which the email monitoring configuration is deleted.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-email-monitoring-configuration-request-schema.json\",\n  \"description\": \"DeleteEmailMonitoringConfigurationRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-email-monitoring-configuration-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DeleteEmailMonitoringConfigurationRequest
---
