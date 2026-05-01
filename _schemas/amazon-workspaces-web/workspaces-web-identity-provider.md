---
description: The identity provider.
layout: schema
name: IdentityProvider
properties_list:
- description: ''
  name: identityProviderArn
  type: object
- description: ''
  name: identityProviderDetails
  type: object
- description: ''
  name: identityProviderName
  type: object
- description: ''
  name: identityProviderType
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-identity-provider-schema.json
slug: workspaces-web-identity-provider
source_filename: workspaces-web-identity-provider-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"identityProviderArn\"\n  ],\n  \"properties\": {\n    \"identityProviderArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the identity provider.\"\n        }\n      ]\n    },\n    \"identityProviderDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProviderDetails\"\n        },\n        {\n          \"description\": \"<p>The identity provider details. The following list describes the provider detail keys for each identity provider type. </p> <ul> <li> <p>For Google and Login with Amazon:</p> <ul> <li> <p> <code>client_id</code> </p> </li> <li> <p> <code>client_secret</code> </p> </li> <li> <p> <code>authorize_scopes</code> </p> </li> </ul> </li> <li> <p>For Facebook:</p> <ul> <li> <p> <code>client_id</code> </p> </li> <li> <p> <code>client_secret</code> </p> </li> <li> <p> <code>authorize_scopes</code>\
  \ </p> </li> <li> <p> <code>api_version</code> </p> </li> </ul> </li> <li> <p>For Sign in with Apple:</p> <ul> <li> <p> <code>client_id</code> </p> </li> <li> <p> <code>team_id</code> </p> </li> <li> <p> <code>key_id</code> </p> </li> <li> <p> <code>private_key</code> </p> </li> <li> <p> <code>authorize_scopes</code> </p> </li> </ul> </li> <li> <p>For OIDC providers:</p> <ul> <li> <p> <code>client_id</code> </p> </li> <li> <p> <code>client_secret</code> </p> </li> <li> <p> <code>attributes_request_method</code> </p> </li> <li> <p> <code>oidc_issuer</code> </p> </li> <li> <p> <code>authorize_scopes</code> </p> </li> <li> <p> <code>authorize_url</code> <i>if not available from discovery URL specified by oidc_issuer key</i> </p> </li> <li> <p> <code>token_url</code> <i>if not available from discovery URL specified by oidc_issuer key</i> </p> </li> <li> <p> <code>attributes_url</code> <i>if not available from discovery URL specified by oidc_issuer key</i> </p> </li> <li> <p> <code>jwks_uri</code>\
  \ <i>if not available from discovery URL specified by oidc_issuer key</i> </p> </li> </ul> </li> <li> <p>For SAML providers:</p> <ul> <li> <p> <code>MetadataFile</code> OR <code>MetadataURL</code> </p> </li> <li> <p> <code>IDPSignout</code> <i>optional</i> </p> </li> </ul> </li> </ul>\"\n        }\n      ]\n    },\n    \"identityProviderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProviderName\"\n        },\n        {\n          \"description\": \"The identity provider name.\"\n        }\n      ]\n    },\n    \"identityProviderType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProviderType\"\n        },\n        {\n          \"description\": \"The identity provider type.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The identity provider.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IdentityProvider\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-identity-provider-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-identity-provider-schema.json
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: IdentityProvider
---
