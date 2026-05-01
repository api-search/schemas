---
description: UpdatePortalRequest schema from Amazon WorkSpaces Web API
layout: schema
name: UpdatePortalRequest
properties_list:
- description: ''
  name: authenticationType
  type: object
- description: ''
  name: displayName
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-update-portal-request-schema.json
slug: workspaces-web-update-portal-request
source_filename: workspaces-web-update-portal-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"UpdatePortalRequest\",\n  \"properties\": {\n    \"authenticationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationType\"\n        },\n        {\n          \"description\": \"<p>The type of authentication integration points used when signing into the web portal. Defaults to <code>Standard</code>.</p> <p> <code>Standard</code> web portals are authenticated directly through your identity provider. You need to call <code>CreateIdentityProvider</code> to integrate your identity provider with your web portal. User and group access to your web portal is controlled through your identity provider.</p> <p> <code>IAM_Identity_Center</code> web portals are authenticated through AWS IAM Identity Center (successor to AWS Single Sign-On). They provide additional features, such as IdP-initiated authentication. Identity sources (including external identity provider integration), plus user and group\
  \ access to your web portal, can be configured in the IAM Identity Center.</p>\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisplayName\"\n        },\n        {\n          \"description\": \"The name of the web portal. This is not visible to users who log into the web portal.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-update-portal-request-schema.json\",\n  \"description\": \"UpdatePortalRequest schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-update-portal-request-schema.json
tags:
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: UpdatePortalRequest
---
