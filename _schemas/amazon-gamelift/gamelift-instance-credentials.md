---
description: Set of credentials required to remotely access a fleet instance.
layout: schema
name: InstanceCredentials
properties_list:
- description: ''
  name: UserName
  type: object
- description: ''
  name: Secret
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-instance-credentials-schema.json
slug: gamelift-instance-credentials
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-instance-credentials-schema.json\",\n  \"title\": \"InstanceCredentials\",\n  \"description\": \"Set of credentials required to remotely access a fleet instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"User login string.\"\n        }\n      ]\n    },\n    \"Secret\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"Secret string. For Windows instances, the secret is a password for use with Windows Remote Desktop. For Linux instances, it is a private key (which must be saved as a <code>.pem</code> file) for use with SSH.\"\n \
  \       }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-instance-credentials-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: InstanceCredentials
---
