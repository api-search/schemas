---
description: List all the <code>AvailabilityConfiguration</code>'s for the given WorkMail organization.
layout: schema
name: AvailabilityConfiguration
properties_list:
- description: ''
  name: DomainName
  type: object
- description: ''
  name: ProviderType
  type: object
- description: ''
  name: EwsProvider
  type: object
- description: ''
  name: LambdaProvider
  type: object
- description: ''
  name: DateCreated
  type: object
- description: ''
  name: DateModified
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-availability-configuration-schema.json
slug: workmail-availability-configuration
source_filename: workmail-availability-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"Displays the domain to which the provider applies.\"\n        }\n      ]\n    },\n    \"ProviderType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailabilityProviderType\"\n        },\n        {\n          \"description\": \"Displays the provider type that applies to this domain.\"\n        }\n      ]\n    },\n    \"EwsProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RedactedEwsAvailabilityProvider\"\n        },\n        {\n          \"description\": \"If <code>ProviderType</code> is <code>EWS</code>, then this field contains <code>RedactedEwsAvailabilityProvider</code>. Otherwise, it is not required.\"\n        }\n      ]\n    },\n    \"LambdaProvider\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/LambdaAvailabilityProvider\"\n        },\n        {\n          \"description\": \"If ProviderType is <code>LAMBDA</code> then this field contains <code>LambdaAvailabilityProvider</code>. Otherwise, it is not required.\"\n        }\n      ]\n    },\n    \"DateCreated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time at which the availability configuration was created.\"\n        }\n      ]\n    },\n    \"DateModified\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time at which the availability configuration was last modified.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"List all the <code>AvailabilityConfiguration</code>'s for the given WorkMail organization.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"AvailabilityConfiguration\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-availability-configuration-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-availability-configuration-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: AvailabilityConfiguration
---
