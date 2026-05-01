---
description: TestAvailabilityConfigurationRequest schema from Amazon WorkMail API
layout: schema
name: TestAvailabilityConfigurationRequest
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
schema_file: json-schema/workmail-test-availability-configuration-request-schema.json
slug: workmail-test-availability-configuration-request
source_filename: workmail-test-availability-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\"\n  ],\n  \"title\": \"TestAvailabilityConfigurationRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The WorkMail organization where the availability provider will be tested.\"\n        }\n      ]\n    },\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The domain to which the provider applies. If this field is provided, a stored availability provider associated to this domain name will be tested.\"\n        }\n      ]\n    },\n    \"EwsProvider\": {\n      \"$ref\": \"#/components/schemas/EwsAvailabilityProvider\"\n    },\n    \"LambdaProvider\": {\n      \"$ref\": \"#/components/schemas/LambdaAvailabilityProvider\"\n    }\n  },\n  \"$schema\"\
  : \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-test-availability-configuration-request-schema.json\",\n  \"description\": \"TestAvailabilityConfigurationRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-test-availability-configuration-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: TestAvailabilityConfigurationRequest
---
