---
description: Organization Config rule creation or deletion status in each member account. This includes the name of the rule, the status, error code and error message when the rule creation or deletion failed.
layout: schema
name: MemberAccountStatus
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: ConfigRuleName
  type: object
- description: ''
  name: MemberAccountRuleStatus
  type: object
- description: ''
  name: ErrorCode
  type: object
- description: ''
  name: ErrorMessage
  type: object
- description: ''
  name: LastUpdateTime
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-member-account-status-schema.json
slug: config-member-account-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-member-account-status-schema.json\",\n  \"title\": \"MemberAccountStatus\",\n  \"description\": \"Organization Config rule creation or deletion status in each member account. This includes the name of the rule, the status, error code and error message when the rule creation or deletion failed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit account ID of a member account.\"\n        }\n      ]\n    },\n    \"ConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit64\"\n        },\n        {\n          \"description\": \"The name of Config rule deployed in the member account.\"\
  \n        }\n      ]\n    },\n    \"MemberAccountRuleStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberAccountRuleStatus\"\n        },\n        {\n          \"description\": \"<p>Indicates deployment status for Config rule in the member account. When management account calls <code>PutOrganizationConfigRule</code> action for the first time, Config rule status is created in the member account. When management account calls <code>PutOrganizationConfigRule</code> action for the second time, Config rule status is updated in the member account. Config rule status is deleted when the management account deletes <code>OrganizationConfigRule</code> and disables service access for <code>config-multiaccountsetup.amazonaws.com</code>. </p> <p> Config sets the state of the rule to:</p> <ul> <li> <p> <code>CREATE_SUCCESSFUL</code> when Config rule has been created in the member account. </p> </li> <li> <p> <code>CREATE_IN_PROGRESS</code> when Config rule is\
  \ being created in the member account.</p> </li> <li> <p> <code>CREATE_FAILED</code> when Config rule creation has failed in the member account.</p> </li> <li> <p> <code>DELETE_FAILED</code> when Config rule deletion has failed in the member account.</p> </li> <li> <p> <code>DELETE_IN_PROGRESS</code> when Config rule is being deleted in the member account.</p> </li> <li> <p> <code>DELETE_SUCCESSFUL</code> when Config rule has been deleted in the member account. </p> </li> <li> <p> <code>UPDATE_SUCCESSFUL</code> when Config rule has been updated in the member account.</p> </li> <li> <p> <code>UPDATE_IN_PROGRESS</code> when Config rule is being updated in the member account.</p> </li> <li> <p> <code>UPDATE_FAILED</code> when Config rule deletion has failed in the member account.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"An error\
  \ code that is returned when Config rule creation or deletion failed in the member account.\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"An error message indicating that Config rule account creation or deletion has failed due to an error in the member account.\"\n        }\n      ]\n    },\n    \"LastUpdateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The timestamp of the last status update.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccountId\",\n    \"ConfigRuleName\",\n    \"MemberAccountRuleStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-member-account-status-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: MemberAccountStatus
---
