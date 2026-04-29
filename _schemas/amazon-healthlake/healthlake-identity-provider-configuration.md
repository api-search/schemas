---
description: The identity provider configuration that you gave when the data store was created.
layout: schema
name: IdentityProviderConfiguration
properties_list:
- description: ''
  name: AuthorizationStrategy
  type: object
- description: ''
  name: FineGrainedAuthorizationEnabled
  type: object
- description: ''
  name: Metadata
  type: object
- description: ''
  name: IdpLambdaArn
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-identity-provider-configuration-schema.json
slug: healthlake-identity-provider-configuration
source_filename: healthlake-identity-provider-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-identity-provider-configuration-schema.json\",\n  \"title\": \"IdentityProviderConfiguration\",\n  \"type\": \"object\",\n  \"required\": [\n    \"AuthorizationStrategy\"\n  ],\n  \"properties\": {\n    \"AuthorizationStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthorizationStrategy\"\n        },\n        {\n          \"description\": \"The authorization strategy that you selected when you created the data store.\"\n        }\n      ]\n    },\n    \"FineGrainedAuthorizationEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"If you enabled fine-grained authorization when you created the data store.\"\n        }\n      ]\n    },\n    \"Metadata\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationMetadata\"\n        },\n        {\n          \"description\": \"<p>The JSON metadata elements that you want to use in your identity provider configuration. Required elements are listed based on the launch specification of the SMART application. For more information on all possible elements, see <a href=\\\"https://build.fhir.org/ig/HL7/smart-app-launch/conformance.html#metadata\\\">Metadata</a> in SMART's App Launch specification.</p> <p> <code>authorization_endpoint</code>: The URL to the OAuth2 authorization endpoint.</p> <p> <code>grant_types_supported</code>: An array of grant types that are supported at the token endpoint. You must provide at least one grant type option. Valid options are <code>authorization_code</code> and <code>client_credentials</code>.</p> <p> <code>token_endpoint</code>: The URL to the OAuth2 token endpoint.</p> <p> <code>capabilities</code>: An array of strings of the SMART\
  \ capabilities that the authorization server supports.</p> <p> <code>code_challenge_methods_supported</code>: An array of strings of supported PKCE code challenge methods. You must include the <code>S256</code> method in the array of PKCE code challenge methods.</p>\"\n        }\n      ]\n    },\n    \"IdpLambdaArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Lambda function that you want to use to decode the access token created by the authorization server.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The identity provider configuration that you gave when the data store was created.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-identity-provider-configuration-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: IdentityProviderConfiguration
---
