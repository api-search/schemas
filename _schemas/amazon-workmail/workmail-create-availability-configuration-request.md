---
description: CreateAvailabilityConfigurationRequest schema from Amazon WorkMail API
layout: schema
name: CreateAvailabilityConfigurationRequest
properties_list:
- description: ''
  name: ClientToken
  type: object
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
schema_file: json-schema/workmail-create-availability-configuration-request-schema.json
slug: workmail-create-availability-configuration-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"DomainName\"\n  ],\n  \"title\": \"CreateAvailabilityConfigurationRequest\",\n  \"properties\": {\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyClientToken\"\n        },\n        {\n          \"description\": \"An idempotent token that ensures that an API request is executed only once.\"\n        }\n      ]\n    },\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The WorkMail organization for which the <code>AvailabilityConfiguration</code> will be created.\"\n        }\n      ]\n    },\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The domain to which the provider applies.\"\n        }\n      ]\n \
  \   },\n    \"EwsProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EwsAvailabilityProvider\"\n        },\n        {\n          \"description\": \"Exchange Web Services (EWS) availability provider definition. The request must contain exactly one provider definition, either <code>EwsProvider</code> or <code>LambdaProvider</code>.\"\n        }\n      ]\n    },\n    \"LambdaProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaAvailabilityProvider\"\n        },\n        {\n          \"description\": \"Lambda availability provider definition. The request must contain exactly one provider definition, either <code>EwsProvider</code> or <code>LambdaProvider</code>.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-create-availability-configuration-request-schema.json\"\
  ,\n  \"description\": \"CreateAvailabilityConfigurationRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-create-availability-configuration-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: CreateAvailabilityConfigurationRequest
---
