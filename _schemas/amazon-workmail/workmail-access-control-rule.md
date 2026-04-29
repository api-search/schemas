---
description: A rule that controls access to an WorkMail organization.
layout: schema
name: AccessControlRule
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
  name: DateCreated
  type: object
- description: ''
  name: DateModified
  type: object
- description: ''
  name: ImpersonationRoleIds
  type: object
- description: ''
  name: NotImpersonationRoleIds
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-access-control-rule-schema.json
slug: workmail-access-control-rule
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessControlRuleName\"\n        },\n        {\n          \"description\": \"The rule name.\"\n        }\n      ]\n    },\n    \"Effect\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessControlRuleEffect\"\n        },\n        {\n          \"description\": \"The rule effect.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessControlRuleDescription\"\n        },\n        {\n          \"description\": \"The rule description.\"\n        }\n      ]\n    },\n    \"IpRanges\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpRangeList\"\n        },\n        {\n          \"description\": \"IPv4 CIDR ranges to include in the rule.\"\n        }\n      ]\n    },\n    \"NotIpRanges\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/IpRangeList\"\n        },\n        {\n          \"description\": \"IPv4 CIDR ranges to exclude from the rule.\"\n        }\n      ]\n    },\n    \"Actions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionsList\"\n        },\n        {\n          \"description\": \"Access protocol actions to include in the rule. Valid values include <code>ActiveSync</code>, <code>AutoDiscover</code>, <code>EWS</code>, <code>IMAP</code>, <code>SMTP</code>, <code>WindowsOutlook</code>, and <code>WebMail</code>.\"\n        }\n      ]\n    },\n    \"NotActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionsList\"\n        },\n        {\n          \"description\": \"Access protocol actions to exclude from the rule. Valid values include <code>ActiveSync</code>, <code>AutoDiscover</code>, <code>EWS</code>, <code>IMAP</code>, <code>SMTP</code>, <code>WindowsOutlook</code>, and\
  \ <code>WebMail</code>.\"\n        }\n      ]\n    },\n    \"UserIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserIdList\"\n        },\n        {\n          \"description\": \"User IDs to include in the rule.\"\n        }\n      ]\n    },\n    \"NotUserIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserIdList\"\n        },\n        {\n          \"description\": \"User IDs to exclude from the rule.\"\n        }\n      ]\n    },\n    \"DateCreated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date that the rule was created.\"\n        }\n      ]\n    },\n    \"DateModified\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date that the rule was modified.\"\n        }\n      ]\n    },\n    \"ImpersonationRoleIds\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleIdList\"\n        },\n        {\n          \"description\": \"Impersonation role IDs to include in the rule.\"\n        }\n      ]\n    },\n    \"NotImpersonationRoleIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpersonationRoleIdList\"\n        },\n        {\n          \"description\": \"Impersonation role IDs to exclude from the rule.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A rule that controls access to an WorkMail organization.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccessControlRule\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-access-control-rule-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-access-control-rule-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: AccessControlRule
---
