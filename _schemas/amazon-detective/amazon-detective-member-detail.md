---
description: Details about a member account in a behavior graph
layout: schema
name: MemberDetail
properties_list:
- description: The AWS account identifier of the member account.
  name: AccountId
  type: string
- description: The AWS account root user email address for the member account.
  name: EmailAddress
  type: string
- description: The ARN of the behavior graph that the member account was invited to.
  name: GraphArn
  type: string
- description: The AWS account identifier of the administrator account for the behavior graph.
  name: AdministratorId
  type: string
- description: The current membership status of the member account.
  name: Status
  type: string
- description: The date and time that Detective sent the invitation to the member account.
  name: InvitedTime
  type: string
- description: The date and time that the member account was last updated.
  name: UpdatedTime
  type: string
- description: Data volume in bytes per day for the member account.
  name: VolumeUsageInBytes
  type: integer
- description: The data and time when the member account data volume was last updated.
  name: VolumeUsageUpdatedTime
  type: string
- description: The member account data volume as a percentage of the maximum allowed data volume.
  name: PercentOfGraphUtilization
  type: number
- description: For member accounts with a status of ACCEPTED_BUT_DISABLED, the reason the member account is not enabled.
  name: DisabledReason
  type: string
- description: The type of behavior graph membership.
  name: InvitationType
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-member-detail-schema.json
slug: amazon-detective-member-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-member-detail-schema.json\",\n  \"title\": \"MemberDetail\",\n  \"description\": \"Details about a member account in a behavior graph\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS account identifier of the member account.\",\n      \"example\": \"234567890123\"\n    },\n    \"EmailAddress\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS account root user email address for the member account.\",\n      \"example\": \"security@example.com\"\n    },\n    \"GraphArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the behavior graph that the member account was invited to.\",\n      \"example\": \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n  \
  \  },\n    \"AdministratorId\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS account identifier of the administrator account for the behavior graph.\",\n      \"example\": \"123456789012\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The current membership status of the member account.\",\n      \"enum\": [\n        \"INVITED\",\n        \"VERIFICATION_IN_PROGRESS\",\n        \"VERIFICATION_FAILED\",\n        \"ENABLED\",\n        \"ACCEPTED_BUT_DISABLED\"\n      ],\n      \"example\": \"ENABLED\"\n    },\n    \"InvitedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time that Detective sent the invitation to the member account.\",\n      \"example\": \"2025-01-15T10:00:00Z\"\n    },\n    \"UpdatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time that the member account was last updated.\",\n      \"example\"\
  : \"2025-01-16T12:00:00Z\"\n    },\n    \"VolumeUsageInBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Data volume in bytes per day for the member account.\",\n      \"example\": 1073741824\n    },\n    \"VolumeUsageUpdatedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The data and time when the member account data volume was last updated.\",\n      \"example\": \"2025-01-16T12:00:00Z\"\n    },\n    \"PercentOfGraphUtilization\": {\n      \"type\": \"number\",\n      \"description\": \"The member account data volume as a percentage of the maximum allowed data volume.\",\n      \"example\": 12.5\n    },\n    \"DisabledReason\": {\n      \"type\": \"string\",\n      \"description\": \"For member accounts with a status of ACCEPTED_BUT_DISABLED, the reason the member account is not enabled.\",\n      \"enum\": [\n        \"VOLUME_TOO_HIGH\",\n        \"VOLUME_UNKNOWN\"\n      ],\n      \"example\": \"VOLUME_TOO_HIGH\"\n\
  \    },\n    \"InvitationType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of behavior graph membership.\",\n      \"enum\": [\n        \"INVITATION\",\n        \"ORGANIZATION\"\n      ],\n      \"example\": \"INVITATION\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-member-detail-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: MemberDetail
---
