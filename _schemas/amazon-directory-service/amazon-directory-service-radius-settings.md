---
description: Contains information about a Remote Authentication Dial In User Service (RADIUS) server.
layout: schema
name: RadiusSettings
properties_list:
- description: ''
  name: RadiusServers
  type: object
- description: ''
  name: RadiusPort
  type: object
- description: ''
  name: RadiusTimeout
  type: object
- description: ''
  name: RadiusRetries
  type: object
- description: ''
  name: SharedSecret
  type: object
- description: ''
  name: AuthenticationProtocol
  type: object
- description: ''
  name: DisplayLabel
  type: object
- description: ''
  name: UseSameUsername
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-radius-settings-schema.json
slug: amazon-directory-service-radius-settings
source_filename: amazon-directory-service-radius-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-radius-settings-schema.json\",\n  \"title\": \"RadiusSettings\",\n  \"description\": \"Contains information about a Remote Authentication Dial In User Service (RADIUS) server.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RadiusServers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Servers\"\n        },\n        {\n          \"description\": \"An array of strings that contains the fully qualified domain name (FQDN) or IP addresses of the RADIUS server endpoints, or the FQDN or IP addresses of your RADIUS server load balancer.\"\n        }\n      ]\n    },\n    \"RadiusPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortNumber\"\n        },\n        {\n          \"description\": \"The port that\
  \ your RADIUS server is using for communications. Your self-managed network must allow inbound traffic over this port from the Directory Service servers.\"\n        }\n      ]\n    },\n    \"RadiusTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RadiusTimeout\"\n        },\n        {\n          \"description\": \"The amount of time, in seconds, to wait for the RADIUS server to respond.\"\n        }\n      ]\n    },\n    \"RadiusRetries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RadiusRetries\"\n        },\n        {\n          \"description\": \"The maximum number of times that communication with the RADIUS server is attempted.\"\n        }\n      ]\n    },\n    \"SharedSecret\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RadiusSharedSecret\"\n        },\n        {\n          \"description\": \"Required for enabling RADIUS on the directory.\"\n        }\n      ]\n    },\n    \"\
  AuthenticationProtocol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RadiusAuthenticationProtocol\"\n        },\n        {\n          \"description\": \"The protocol specified for your RADIUS endpoints.\"\n        }\n      ]\n    },\n    \"DisplayLabel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RadiusDisplayLabel\"\n        },\n        {\n          \"description\": \"Not currently used.\"\n        }\n      ]\n    },\n    \"UseSameUsername\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UseSameUsername\"\n        },\n        {\n          \"description\": \"Not currently used.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-radius-settings-schema.json
tags:
- Active Directory
- Authentication
- Directory Services
- Identity Management
title: RadiusSettings
---
