---
description: The compromised credentials risk configuration type.
layout: schema
name: CompromisedCredentialsRiskConfigurationType
properties_list:
- description: ''
  name: EventFilter
  type: object
- description: ''
  name: Actions
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-compromised-credentials-risk-configuration-type-schema.json
slug: user-pools-compromised-credentials-risk-configuration-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-compromised-credentials-risk-configuration-type-schema.json\",\n  \"title\": \"CompromisedCredentialsRiskConfigurationType\",\n  \"description\": \"The compromised credentials risk configuration type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EventFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventFiltersType\"\n        },\n        {\n          \"description\": \"Perform the action for these events. The default is to perform all events if no event filter is specified.\"\n        }\n      ]\n    },\n    \"Actions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CompromisedCredentialsActionsType\"\n        },\n        {\n          \"description\": \"The compromised credentials risk configuration actions.\"\n \
  \       }\n      ]\n    }\n  },\n  \"required\": [\n    \"Actions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-compromised-credentials-risk-configuration-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: CompromisedCredentialsRiskConfigurationType
---
