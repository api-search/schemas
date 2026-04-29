---
description: Describes the enablement status, user access URL, and relay state parameter name that are used for configuring federation with an SAML 2.0 identity provider.
layout: schema
name: SamlProperties
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: UserAccessUrl
  type: object
- description: ''
  name: RelayStateParameterName
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-saml-properties-schema.json
slug: workspaces-saml-properties
source_filename: workspaces-saml-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamlStatusEnum\"\n        },\n        {\n          \"description\": \"<p>Indicates the status of SAML 2.0 authentication. These statuses include the following.</p> <ul> <li> <p>If the setting is <code>DISABLED</code>, end users will be directed to login with their directory credentials.</p> </li> <li> <p>If the setting is <code>ENABLED</code>, end users will be directed to login via the user access URL. Users attempting to connect to WorkSpaces from a client application that does not support SAML 2.0 authentication will not be able to connect.</p> </li> <li> <p>If the setting is <code>ENABLED_WITH_DIRECTORY_LOGIN_FALLBACK</code>, end users will be directed to login via the user access URL on supported client applications, but will not prevent clients that do not support SAML 2.0 authentication from connecting as if SAML 2.0 authentication\
  \ was disabled.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"UserAccessUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamlUserAccessUrl\"\n        },\n        {\n          \"description\": \"The SAML 2.0 identity provider (IdP) user access URL is the URL a user would navigate to in their web browser in order to federate from the IdP and directly access the application, without any SAML 2.0 service provider (SP) bindings.\"\n        }\n      ]\n    },\n    \"RelayStateParameterName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"<p>The relay state parameter name supported by the SAML 2.0 identity provider (IdP). When the end user is redirected to the user access URL from the WorkSpaces client application, this relay state parameter name is appended as a query parameter to the URL along with the relay state endpoint to return the user to the client\
  \ application session.</p> <p>To use SAML 2.0 authentication with WorkSpaces, the IdP must support IdP-initiated deep linking for the relay state URL. Consult your IdP documentation for more information.</p>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes the enablement status, user access URL, and relay state parameter name that are used for configuring federation with an SAML 2.0 identity provider.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SamlProperties\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-saml-properties-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-saml-properties-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: SamlProperties
---
