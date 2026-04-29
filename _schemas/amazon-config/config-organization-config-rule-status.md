---
description: Returns the status for an organization Config rule in an organization.
layout: schema
name: OrganizationConfigRuleStatus
properties_list:
- description: ''
  name: OrganizationConfigRuleName
  type: object
- description: ''
  name: OrganizationRuleStatus
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
schema_file: json-schema/config-organization-config-rule-status-schema.json
slug: config-organization-config-rule-status
source_filename: config-organization-config-rule-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-config-rule-status-schema.json\",\n  \"title\": \"OrganizationConfigRuleStatus\",\n  \"description\": \"Returns the status for an organization Config rule in an organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationConfigRuleName\"\n        },\n        {\n          \"description\": \"The name that you assign to organization Config rule.\"\n        }\n      ]\n    },\n    \"OrganizationRuleStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationRuleStatus\"\n        },\n        {\n          \"description\": \"<p>Indicates deployment status of an organization Config rule. When management account calls PutOrganizationConfigRule\
  \ action for the first time, Config rule status is created in all the member accounts. When management account calls PutOrganizationConfigRule action for the second time, Config rule status is updated in all the member accounts. Additionally, Config rule status is updated when one or more member accounts join or leave an organization. Config rule status is deleted when the management account deletes OrganizationConfigRule in all the member accounts and disables service access for <code>config-multiaccountsetup.amazonaws.com</code>.</p> <p>Config sets the state of the rule to:</p> <ul> <li> <p> <code>CREATE_SUCCESSFUL</code> when an organization Config rule has been successfully created in all the member accounts. </p> </li> <li> <p> <code>CREATE_IN_PROGRESS</code> when an organization Config rule creation is in progress.</p> </li> <li> <p> <code>CREATE_FAILED</code> when an organization Config rule creation failed in one or more member accounts within that organization.</p> </li> <li>\
  \ <p> <code>DELETE_FAILED</code> when an organization Config rule deletion failed in one or more member accounts within that organization.</p> </li> <li> <p> <code>DELETE_IN_PROGRESS</code> when an organization Config rule deletion is in progress.</p> </li> <li> <p> <code>DELETE_SUCCESSFUL</code> when an organization Config rule has been successfully deleted from all the member accounts.</p> </li> <li> <p> <code>UPDATE_SUCCESSFUL</code> when an organization Config rule has been successfully updated in all the member accounts.</p> </li> <li> <p> <code>UPDATE_IN_PROGRESS</code> when an organization Config rule update is in progress.</p> </li> <li> <p> <code>UPDATE_FAILED</code> when an organization Config rule update failed in one or more member accounts within that organization.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"An error\
  \ code that is returned when organization Config rule creation or deletion has failed.\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"An error message indicating that organization Config rule creation or deletion failed due to an error.\"\n        }\n      ]\n    },\n    \"LastUpdateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The timestamp of the last update.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OrganizationConfigRuleName\",\n    \"OrganizationRuleStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-config-rule-status-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: OrganizationConfigRuleStatus
---
