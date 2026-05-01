---
description: DeleteAvailabilityConfigurationRequest schema from Amazon WorkMail API
layout: schema
name: DeleteAvailabilityConfigurationRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: DomainName
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-delete-availability-configuration-request-schema.json
slug: workmail-delete-availability-configuration-request
source_filename: workmail-delete-availability-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"DomainName\"\n  ],\n  \"title\": \"DeleteAvailabilityConfigurationRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The WorkMail organization for which the <code>AvailabilityConfiguration</code> will be deleted.\"\n        }\n      ]\n    },\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The domain for which the <code>AvailabilityConfiguration</code> will be deleted.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-availability-configuration-request-schema.json\"\
  ,\n  \"description\": \"DeleteAvailabilityConfigurationRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-delete-availability-configuration-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DeleteAvailabilityConfigurationRequest
---
