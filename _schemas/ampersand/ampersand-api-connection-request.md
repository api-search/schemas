---
description: ConnectionRequest schema from Ampersand API
layout: schema
name: ConnectionRequest
properties_list:
- description: The ID of the provider workspace that this connection belongs to.
  name: providerWorkspaceRef
  type: string
- description: ''
  name: providerMetadata
  type: object
- description: The name of the user group that has access to this installation.
  name: groupName
  type: string
- description: The ID of the user group that has access to this installation.
  name: groupRef
  type: string
- description: The name of the consumer that has access to this installation.
  name: consumerName
  type: string
- description: The consumer reference.
  name: consumerRef
  type: string
- description: The provider name (e.g. "salesforce", "hubspot")
  name: provider
  type: string
- description: The API key to use for the connection.
  name: apiKey
  type: string
- description: Values used for custom auth input variables.
  name: customAuth
  type: object
- description: ''
  name: basicAuth
  type: object
- description: ''
  name: oauth2ClientCredentials
  type: object
- description: ''
  name: oauth2PasswordCredentials
  type: object
- description: ''
  name: oauth2AuthorizationCode
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-connection-request-schema.json
slug: ampersand-api-connection-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-connection-request-schema.json\",\n  \"title\": \"ConnectionRequest\",\n  \"description\": \"ConnectionRequest schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"providerWorkspaceRef\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the provider workspace that this connection belongs to.\"\n    },\n    \"providerMetadata\": {\n      \"$ref\": \"#/components/schemas/ProviderMetadata\"\n    },\n    \"groupName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the user group that has access to this installation.\"\n    },\n    \"groupRef\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the user group that has access to this installation.\",\n      \"example\": \"group-123\"\n    },\n    \"consumerName\":\
  \ {\n      \"type\": \"string\",\n      \"description\": \"The name of the consumer that has access to this installation.\"\n    },\n    \"consumerRef\": {\n      \"type\": \"string\",\n      \"description\": \"The consumer reference.\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"The provider name (e.g. \\\"salesforce\\\", \\\"hubspot\\\")\"\n    },\n    \"apiKey\": {\n      \"type\": \"string\",\n      \"description\": \"The API key to use for the connection.\"\n    },\n    \"customAuth\": {\n      \"type\": \"object\",\n      \"description\": \"Values used for custom auth input variables.\",\n      \"additionalProperties\": {\n        \"type\": \"string\",\n        \"nullable\": false\n      },\n      \"example\": {\n        \"apiKey\": \"abcd1234\",\n        \"password\": \"secret\"\n      }\n    },\n    \"basicAuth\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"username\",\n        \"password\"\n      ],\n      \"properties\"\
  : {\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"The username to use for the connection.\"\n        },\n        \"password\": {\n          \"type\": \"string\",\n          \"description\": \"The password to use for the connection.\"\n        }\n      }\n    },\n    \"oauth2ClientCredentials\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"clientId\",\n        \"clientSecret\"\n      ],\n      \"properties\": {\n        \"clientId\": {\n          \"type\": \"string\",\n          \"description\": \"The client ID to use for the connection.\"\n        },\n        \"clientSecret\": {\n          \"type\": \"string\",\n          \"description\": \"The client secret to use for the connection.\"\n        },\n        \"scopes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"The scopes for the tokens.\"\n        }\n      }\n    },\n    \"oauth2PasswordCredentials\"\
  : {\n      \"type\": \"object\",\n      \"required\": [\n        \"username\",\n        \"password\",\n        \"clientId\",\n        \"clientSecret\"\n      ],\n      \"properties\": {\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"The username to use for the connection.\"\n        },\n        \"password\": {\n          \"type\": \"string\",\n          \"description\": \"The password to use for the connection.\"\n        },\n        \"clientId\": {\n          \"type\": \"string\",\n          \"description\": \"The client ID to use for the connection.\"\n        },\n        \"clientSecret\": {\n          \"type\": \"string\",\n          \"description\": \"The client secret to use for the connection.\"\n        },\n        \"scopes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"The scopes for the tokens.\"\n        }\n      }\n    },\n    \"oauth2AuthorizationCode\"\
  : {\n      \"$ref\": \"#/components/schemas/Oauth2AuthorizationCode\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-connection-request-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: ConnectionRequest
---
