---
description: Schema defining the structure of an AWS Organization resource, including accounts, organizational units, policies, and the organization hierarchy.
layout: schema
name: AWS Organizations Definition
properties_list:
- description: The unique identifier of the organization.
  name: Id
  type: string
- description: The Amazon Resource Name of the organization.
  name: Arn
  type: string
- description: Specifies the functionality available to the organization.
  name: FeatureSet
  type: string
- description: The ARN of the management account.
  name: MasterAccountArn
  type: string
- description: The unique identifier of the management account.
  name: MasterAccountId
  type: string
- description: The email address associated with the management account.
  name: MasterAccountEmail
  type: string
- description: A list of policy types enabled for the organization.
  name: AvailablePolicyTypes
  type: array
- description: The member accounts in the organization.
  name: Accounts
  type: array
- description: The organizational units in the organization.
  name: OrganizationalUnits
  type: array
- description: The policies attached in the organization.
  name: Policies
  type: array
- description: The root containers in the organization.
  name: Roots
  type: array
provider_name: Amazon Organizations
provider_slug: amazon-organizations
schema_file: json-schema/amazon-organizations-schema.json
slug: amazon-organizations
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.apievangelist.com/amazon-organizations/organization-definition\",\n  \"title\": \"AWS Organizations Definition\",\n  \"description\": \"Schema defining the structure of an AWS Organization resource, including accounts, organizational units, policies, and the organization hierarchy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the organization.\",\n      \"pattern\": \"^o-[a-z0-9]{10,32}$\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name of the organization.\"\n    },\n    \"FeatureSet\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ALL\",\n        \"CONSOLIDATED_BILLING\"\n      ],\n      \"description\": \"Specifies the functionality available to the organization.\"\n    },\n    \"MasterAccountArn\": {\n    \
  \  \"type\": \"string\",\n      \"description\": \"The ARN of the management account.\"\n    },\n    \"MasterAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the management account.\",\n      \"pattern\": \"^\\\\d{12}$\"\n    },\n    \"MasterAccountEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address associated with the management account.\"\n    },\n    \"AvailablePolicyTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PolicyTypeSummary\"\n      },\n      \"description\": \"A list of policy types enabled for the organization.\"\n    },\n    \"Accounts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Account\"\n      },\n      \"description\": \"The member accounts in the organization.\"\n    },\n    \"OrganizationalUnits\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/OrganizationalUnit\"\
  \n      },\n      \"description\": \"The organizational units in the organization.\"\n    },\n    \"Policies\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Policy\"\n      },\n      \"description\": \"The policies attached in the organization.\"\n    },\n    \"Roots\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Root\"\n      },\n      \"description\": \"The root containers in the organization.\"\n    }\n  },\n  \"$defs\": {\n    \"Account\": {\n      \"type\": \"object\",\n      \"description\": \"An AWS account that is a member of the organization.\",\n      \"properties\": {\n        \"Id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the account.\",\n          \"pattern\": \"^\\\\d{12}$\"\n        },\n        \"Arn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the account.\"\n        },\n        \"Email\": {\n          \"type\": \"string\"\
  ,\n          \"format\": \"email\",\n          \"description\": \"The email address associated with the account.\"\n        },\n        \"Name\": {\n          \"type\": \"string\",\n          \"description\": \"The friendly name of the account.\",\n          \"minLength\": 1,\n          \"maxLength\": 50\n        },\n        \"Status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ACTIVE\",\n            \"SUSPENDED\",\n            \"PENDING_CLOSURE\"\n          ],\n          \"description\": \"The status of the account.\"\n        },\n        \"JoinedMethod\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"INVITED\",\n            \"CREATED\"\n          ],\n          \"description\": \"The method by which the account joined the organization.\"\n        },\n        \"JoinedTimestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date the account became a part of the organization.\"\
  \n        }\n      }\n    },\n    \"OrganizationalUnit\": {\n      \"type\": \"object\",\n      \"description\": \"A container for accounts within a root that enables grouping and policy application.\",\n      \"properties\": {\n        \"Id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the organizational unit.\",\n          \"pattern\": \"^ou-[a-z0-9]{4,32}-[a-z0-9]{8,32}$\"\n        },\n        \"Arn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the organizational unit.\"\n        },\n        \"Name\": {\n          \"type\": \"string\",\n          \"description\": \"The friendly name of the organizational unit.\",\n          \"minLength\": 1,\n          \"maxLength\": 128\n        }\n      }\n    },\n    \"Policy\": {\n      \"type\": \"object\",\n      \"description\": \"A policy that defines controls for your organization.\",\n      \"properties\": {\n        \"PolicySummary\": {\n          \"type\": \"\
  object\",\n          \"properties\": {\n            \"Id\": {\n              \"type\": \"string\",\n              \"description\": \"The unique identifier of the policy.\"\n            },\n            \"Arn\": {\n              \"type\": \"string\",\n              \"description\": \"The ARN of the policy.\"\n            },\n            \"Name\": {\n              \"type\": \"string\",\n              \"description\": \"The friendly name of the policy.\",\n              \"minLength\": 1,\n              \"maxLength\": 128\n            },\n            \"Description\": {\n              \"type\": \"string\",\n              \"description\": \"The description of the policy.\",\n              \"maxLength\": 512\n            },\n            \"Type\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"SERVICE_CONTROL_POLICY\",\n                \"TAG_POLICY\",\n                \"BACKUP_POLICY\",\n                \"AISERVICES_OPT_OUT_POLICY\"\n              ],\n    \
  \          \"description\": \"The type of policy.\"\n            },\n            \"AwsManaged\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether the policy is an AWS-managed policy.\"\n            }\n          }\n        },\n        \"Content\": {\n          \"type\": \"string\",\n          \"description\": \"The text content of the policy.\"\n        }\n      }\n    },\n    \"Root\": {\n      \"type\": \"object\",\n      \"description\": \"The top-level container in the hierarchy of organizational units.\",\n      \"properties\": {\n        \"Id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the root.\",\n          \"pattern\": \"^r-[a-z0-9]{4,32}$\"\n        },\n        \"Arn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the root.\"\n        },\n        \"Name\": {\n          \"type\": \"string\",\n          \"description\": \"The friendly name of the root.\"\n        },\n\
  \        \"PolicyTypes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/PolicyTypeSummary\"\n          }\n        }\n      }\n    },\n    \"PolicyTypeSummary\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"SERVICE_CONTROL_POLICY\",\n            \"TAG_POLICY\",\n            \"BACKUP_POLICY\",\n            \"AISERVICES_OPT_OUT_POLICY\"\n          ]\n        },\n        \"Status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ENABLED\",\n            \"PENDING_ENABLE\",\n            \"PENDING_DISABLE\"\n          ]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-organizations/refs/heads/main/json-schema/amazon-organizations-schema.json
tags:
- Account Management
- AWS
- Consolidated Billing
- Governance
- Multi-Account
- Organizations
- Policies
title: AWS Organizations Definition
---
