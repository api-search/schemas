---
description: AssociateTeamMemberResult schema from AWS CodeStar API
layout: schema
name: AssociateTeamMemberResult
properties_list:
- description: ''
  name: clientRequestToken
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-associate-team-member-result-schema.json
slug: codestar-associate-team-member-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-associate-team-member-result-schema.json\",\n  \"title\": \"AssociateTeamMemberResult\",\n  \"description\": \"AssociateTeamMemberResult schema from AWS CodeStar API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n          \"description\": \"The user- or system-generated token from the initial request that can be used to repeat the request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-associate-team-member-result-schema.json
tags:
- AWS
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: AssociateTeamMemberResult
---
