---
description: UpdateAvailabilityConfigurationRequest schema from Amazon WorkMail API
layout: schema
name: UpdateAvailabilityConfigurationRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: DomainName
  type: object
- description: ''
  name: EwsProvider
  type: object
- description: ''
  name: LambdaProvider
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-update-availability-configuration-request-schema.json
slug: workmail-update-availability-configuration-request
source_filename: workmail-update-availability-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"DomainName\"\n  ],\n  \"title\": \"UpdateAvailabilityConfigurationRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The WorkMail organization for which the <code>AvailabilityConfiguration</code> will be updated.\"\n        }\n      ]\n    },\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The domain to which the provider applies the availability configuration.\"\n        }\n      ]\n    },\n    \"EwsProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EwsAvailabilityProvider\"\n        },\n        {\n          \"description\": \"The EWS availability provider definition. The request must contain exactly\
  \ one provider definition, either <code>EwsProvider</code> or <code>LambdaProvider</code>. The previously stored provider will be overridden by the one provided.\"\n        }\n      ]\n    },\n    \"LambdaProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaAvailabilityProvider\"\n        },\n        {\n          \"description\": \"The Lambda availability provider definition. The request must contain exactly one provider definition, either <code>EwsProvider</code> or <code>LambdaProvider</code>. The previously stored provider will be overridden by the one provided.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-update-availability-configuration-request-schema.json\",\n  \"description\": \"UpdateAvailabilityConfigurationRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-update-availability-configuration-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: UpdateAvailabilityConfigurationRequest
---
