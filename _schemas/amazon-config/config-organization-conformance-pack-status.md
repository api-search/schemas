---
description: Returns the status for an organization conformance pack in an organization.
layout: schema
name: OrganizationConformancePackStatus
properties_list:
- description: ''
  name: OrganizationConformancePackName
  type: object
- description: ''
  name: Status
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
schema_file: json-schema/config-organization-conformance-pack-status-schema.json
slug: config-organization-conformance-pack-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-conformance-pack-status-schema.json\",\n  \"title\": \"OrganizationConformancePackStatus\",\n  \"description\": \"Returns the status for an organization conformance pack in an organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationConformancePackName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationConformancePackName\"\n        },\n        {\n          \"description\": \"The name that you assign to organization conformance pack.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationResourceStatus\"\n        },\n        {\n          \"description\": \"<p>Indicates deployment status of an organization conformance pack. When management account\
  \ calls PutOrganizationConformancePack for the first time, conformance pack status is created in all the member accounts. When management account calls PutOrganizationConformancePack for the second time, conformance pack status is updated in all the member accounts. Additionally, conformance pack status is updated when one or more member accounts join or leave an organization. Conformance pack status is deleted when the management account deletes OrganizationConformancePack in all the member accounts and disables service access for <code>config-multiaccountsetup.amazonaws.com</code>.</p> <p>Config sets the state of the conformance pack to:</p> <ul> <li> <p> <code>CREATE_SUCCESSFUL</code> when an organization conformance pack has been successfully created in all the member accounts. </p> </li> <li> <p> <code>CREATE_IN_PROGRESS</code> when an organization conformance pack creation is in progress.</p> </li> <li> <p> <code>CREATE_FAILED</code> when an organization conformance pack creation\
  \ failed in one or more member accounts within that organization.</p> </li> <li> <p> <code>DELETE_FAILED</code> when an organization conformance pack deletion failed in one or more member accounts within that organization.</p> </li> <li> <p> <code>DELETE_IN_PROGRESS</code> when an organization conformance pack deletion is in progress.</p> </li> <li> <p> <code>DELETE_SUCCESSFUL</code> when an organization conformance pack has been successfully deleted from all the member accounts.</p> </li> <li> <p> <code>UPDATE_SUCCESSFUL</code> when an organization conformance pack has been successfully updated in all the member accounts.</p> </li> <li> <p> <code>UPDATE_IN_PROGRESS</code> when an organization conformance pack update is in progress.</p> </li> <li> <p> <code>UPDATE_FAILED</code> when an organization conformance pack update failed in one or more member accounts within that organization.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"An error code that is returned when organization conformance pack creation or deletion has failed in a member account. \"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"An error message indicating that organization conformance pack creation or deletion failed due to an error. \"\n        }\n      ]\n    },\n    \"LastUpdateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The timestamp of the last update.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OrganizationConformancePackName\",\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-conformance-pack-status-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: OrganizationConformancePackStatus
---
