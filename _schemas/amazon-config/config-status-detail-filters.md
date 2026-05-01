---
description: Status filter object to filter results based on specific member account ID or status type for an organization Config rule.
layout: schema
name: StatusDetailFilters
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: MemberAccountRuleStatus
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-status-detail-filters-schema.json
slug: config-status-detail-filters
source_filename: config-status-detail-filters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-status-detail-filters-schema.json\",\n  \"title\": \"StatusDetailFilters\",\n  \"description\": \"Status filter object to filter results based on specific member account ID or status type for an organization Config rule. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit account ID of the member account within an organization.\"\n        }\n      ]\n    },\n    \"MemberAccountRuleStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemberAccountRuleStatus\"\n        },\n        {\n          \"description\": \"<p>Indicates deployment status for Config rule in the member account. When management\
  \ account calls <code>PutOrganizationConfigRule</code> action for the first time, Config rule status is created in the member account. When management account calls <code>PutOrganizationConfigRule</code> action for the second time, Config rule status is updated in the member account. Config rule status is deleted when the management account deletes <code>OrganizationConfigRule</code> and disables service access for <code>config-multiaccountsetup.amazonaws.com</code>. </p> <p>Config sets the state of the rule to:</p> <ul> <li> <p> <code>CREATE_SUCCESSFUL</code> when Config rule has been created in the member account.</p> </li> <li> <p> <code>CREATE_IN_PROGRESS</code> when Config rule is being created in the member account.</p> </li> <li> <p> <code>CREATE_FAILED</code> when Config rule creation has failed in the member account.</p> </li> <li> <p> <code>DELETE_FAILED</code> when Config rule deletion has failed in the member account.</p> </li> <li> <p> <code>DELETE_IN_PROGRESS</code> when\
  \ Config rule is being deleted in the member account.</p> </li> <li> <p> <code>DELETE_SUCCESSFUL</code> when Config rule has been deleted in the member account.</p> </li> <li> <p> <code>UPDATE_SUCCESSFUL</code> when Config rule has been updated in the member account.</p> </li> <li> <p> <code>UPDATE_IN_PROGRESS</code> when Config rule is being updated in the member account.</p> </li> <li> <p> <code>UPDATE_FAILED</code> when Config rule deletion has failed in the member account.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-status-detail-filters-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: StatusDetailFilters
---
