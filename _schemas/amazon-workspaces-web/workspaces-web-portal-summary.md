---
description: The summary of the portal.
layout: schema
name: PortalSummary
properties_list:
- description: ''
  name: authenticationType
  type: object
- description: ''
  name: browserSettingsArn
  type: object
- description: ''
  name: browserType
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: displayName
  type: object
- description: ''
  name: ipAccessSettingsArn
  type: object
- description: ''
  name: networkSettingsArn
  type: object
- description: ''
  name: portalArn
  type: object
- description: ''
  name: portalEndpoint
  type: object
- description: ''
  name: portalStatus
  type: object
- description: ''
  name: rendererType
  type: object
- description: ''
  name: trustStoreArn
  type: object
- description: ''
  name: userAccessLoggingSettingsArn
  type: object
- description: ''
  name: userSettingsArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-portal-summary-schema.json
slug: workspaces-web-portal-summary
source_filename: workspaces-web-portal-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"authenticationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationType\"\n        },\n        {\n          \"description\": \"<p>The type of authentication integration points used when signing into the web portal. Defaults to <code>Standard</code>.</p> <p> <code>Standard</code> web portals are authenticated directly through your identity provider. You need to call <code>CreateIdentityProvider</code> to integrate your identity provider with your web portal. User and group access to your web portal is controlled through your identity provider.</p> <p> <code>IAM_Identity_Center</code> web portals are authenticated through AWS IAM Identity Center (successor to AWS Single Sign-On). They provide additional features, such as IdP-initiated authentication. Identity sources (including external identity provider integration), plus user and group access to your web portal, can be configured\
  \ in the IAM Identity Center.</p>\"\n        }\n      ]\n    },\n    \"browserSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the browser settings that is associated with the web portal.\"\n        }\n      ]\n    },\n    \"browserType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BrowserType\"\n        },\n        {\n          \"description\": \"The browser type of the web portal.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The creation date of the web portal.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisplayName\"\n        },\n        {\n          \"description\": \"The name of the web portal.\"\n       \
  \ }\n      ]\n    },\n    \"ipAccessSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the IP access settings.\"\n        }\n      ]\n    },\n    \"networkSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the network settings that is associated with the web portal.\"\n        }\n      ]\n    },\n    \"portalArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the web portal.\"\n        }\n      ]\n    },\n    \"portalEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortalEndpoint\"\n        },\n        {\n          \"description\": \"The endpoint URL of the web portal that users access in order to start streaming sessions.\"\n \
  \       }\n      ]\n    },\n    \"portalStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortalStatus\"\n        },\n        {\n          \"description\": \"The status of the web portal.\"\n        }\n      ]\n    },\n    \"rendererType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RendererType\"\n        },\n        {\n          \"description\": \"The renderer that is used in streaming sessions.\"\n        }\n      ]\n    },\n    \"trustStoreArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the trust that is associated with this web portal.\"\n        }\n      ]\n    },\n    \"userAccessLoggingSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the user access logging settings that is associated with the\
  \ web portal.\"\n        }\n      ]\n    },\n    \"userSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the user settings that is associated with the web portal.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The summary of the portal.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PortalSummary\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-portal-summary-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-portal-summary-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: PortalSummary
---
