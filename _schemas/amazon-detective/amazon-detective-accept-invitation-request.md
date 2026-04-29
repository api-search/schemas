---
description: Request to accept an invitation to a behavior graph
layout: schema
name: AcceptInvitationRequest
properties_list:
- description: The ARN of the behavior graph that the member account is accepting the invitation for.
  name: GraphArn
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-accept-invitation-request-schema.json
slug: amazon-detective-accept-invitation-request
source_filename: amazon-detective-accept-invitation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-accept-invitation-request-schema.json\",\n  \"title\": \"AcceptInvitationRequest\",\n  \"description\": \"Request to accept an invitation to a behavior graph\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the behavior graph that the member account is accepting the invitation for.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n    }\n  },\n  \"required\": [\n    \"GraphArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-accept-invitation-request-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: AcceptInvitationRequest
---
