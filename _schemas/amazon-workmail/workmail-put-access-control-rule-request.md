---
description: PutAccessControlRuleRequest schema from Amazon WorkMail API
layout: schema
name: PutAccessControlRuleRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Effect
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: IpRanges
  type: object
- description: ''
  name: NotIpRanges
  type: object
- description: ''
  name: Actions
  type: object
- description: ''
  name: NotActions
  type: object
- description: ''
  name: UserIds
  type: object
- description: ''
  name: NotUserIds
  type: object
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: ImpersonationRoleIds
  type: object
- description: ''
  name: NotImpersonationRoleIds
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-put-access-control-rule-request-schema.json
slug: workmail-put-access-control-rule-request
source_filename: workmail-put-access-control-rule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"Name\",\n    \"Effect\",\n    \"Description\",\n    \"OrganizationId\"\n  ],\n  \"title\": \"PutAccessControlRuleRequest\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessControlRuleName\"\n        },\n        {\n          \"description\": \"The rule name.\"\n        }\n      ]\n    },\n    \"Effect\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessControlRuleEffect\"\n        },\n        {\n          \"description\": \"The rule effect.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessControlRuleDescription\"\n        },\n        {\n          \"description\": \"The rule description.\"\n        }\n      ]\n    },\n    \"IpRanges\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpRangeList\"\n        },\n\
  \        {\n          \"description\": \"IPv4 CIDR ranges to include in the rule.\"\n        }\n      ]\n    },\n    \"NotIpRanges\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpRangeList\"\n        },\n        {\n          \"description\": \"IPv4 CIDR ranges to exclude from the rule.\"\n        }\n      ]\n    },\n    \"Actions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionsList\"\n        },\n        {\n          \"description\": \"Access protocol actions to include in the rule. Valid values include <code>ActiveSync</code>, <code>AutoDiscover</code>, <code>EWS</code>, <code>IMAP</code>, <code>SMTP</code>, <code>WindowsOutlook</code>, and <code>WebMail</code>.\"\n        }\n      ]\n    },\n    \"NotActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionsList\"\n        },\n        {\n          \"description\": \"Access protocol actions to exclude from the rule. Valid values\
  \ include <code>ActiveSync</code>, <code>AutoDiscover</code>, <code>EWS</code>, <code>IMAP</code>, <code>SMTP</code>, <code>WindowsOutlook</code>, and <code>WebMail</code>.\"\n        }\n      ]\n    },\n    \"UserIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserIdList\"\n        },\n        {\n          \"description\": \"User IDs to include in the rule.\"\n        }\n      ]\n    },\n    \"NotUserIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserIdList\"\n        },\n        {\n          \"description\": \"User IDs to exclude from the rule.\"\n        }\n      ]\n    },\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier of the organization.\"\n        }\n      ]\n    },\n    \"ImpersonationRoleIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleIdList\"\
  \n        },\n        {\n          \"description\": \"Impersonation role IDs to include in the rule.\"\n        }\n      ]\n    },\n    \"NotImpersonationRoleIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleIdList\"\n        },\n        {\n          \"description\": \"Impersonation role IDs to exclude from the rule.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-put-access-control-rule-request-schema.json\",\n  \"description\": \"PutAccessControlRuleRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-put-access-control-rule-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: PutAccessControlRuleRequest
---
