---
description: The IP access settings resource that can be associated with a web portal.
layout: schema
name: IpAccessSettings
properties_list:
- description: ''
  name: associatedPortalArns
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: displayName
  type: object
- description: ''
  name: ipAccessSettingsArn
  type: object
- description: ''
  name: ipRules
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-ip-access-settings-schema.json
slug: workspaces-web-ip-access-settings
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ipAccessSettingsArn\"\n  ],\n  \"properties\": {\n    \"associatedPortalArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnList\"\n        },\n        {\n          \"description\": \"A list of web portal ARNs that this IP access settings resource is associated with.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The creation date timestamp of the IP access settings.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the IP access settings.\"\n        }\n      ]\n    },\n    \"displayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisplayName\"\
  \n        },\n        {\n          \"description\": \" The display name of the IP access settings.\"\n        }\n      ]\n    },\n    \"ipAccessSettingsArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the IP access settings resource.\"\n        }\n      ]\n    },\n    \"ipRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpRuleList\"\n        },\n        {\n          \"description\": \"The IP rules of the IP access settings.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The IP access settings resource that can be associated with a web portal. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IpAccessSettings\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-ip-access-settings-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-ip-access-settings-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: IpAccessSettings
---
