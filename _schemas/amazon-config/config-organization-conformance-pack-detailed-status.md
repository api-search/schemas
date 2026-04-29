---
description: Organization conformance pack creation or deletion status in each member account. This includes the name of the conformance pack, the status, error code and error message when the conformance pack creation or deletion failed.
layout: schema
name: OrganizationConformancePackDetailedStatus
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: ConformancePackName
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
schema_file: json-schema/config-organization-conformance-pack-detailed-status-schema.json
slug: config-organization-conformance-pack-detailed-status
source_filename: config-organization-conformance-pack-detailed-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-conformance-pack-detailed-status-schema.json\",\n  \"title\": \"OrganizationConformancePackDetailedStatus\",\n  \"description\": \"Organization conformance pack creation or deletion status in each member account. This includes the name of the conformance pack, the status, error code and error message when the conformance pack creation or deletion failed. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit account ID of a member account.\"\n        }\n      ]\n    },\n    \"ConformancePackName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n     \
  \   {\n          \"description\": \"The name of conformance pack deployed in the member account.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationResourceDetailedStatus\"\n        },\n        {\n          \"description\": \"<p>Indicates deployment status for conformance pack in a member account. When management account calls <code>PutOrganizationConformancePack</code> action for the first time, conformance pack status is created in the member account. When management account calls <code>PutOrganizationConformancePack</code> action for the second time, conformance pack status is updated in the member account. Conformance pack status is deleted when the management account deletes <code>OrganizationConformancePack</code> and disables service access for <code>config-multiaccountsetup.amazonaws.com</code>. </p> <p> Config sets the state of the conformance pack to:</p> <ul> <li> <p> <code>CREATE_SUCCESSFUL</code>\
  \ when conformance pack has been created in the member account. </p> </li> <li> <p> <code>CREATE_IN_PROGRESS</code> when conformance pack is being created in the member account.</p> </li> <li> <p> <code>CREATE_FAILED</code> when conformance pack creation has failed in the member account.</p> </li> <li> <p> <code>DELETE_FAILED</code> when conformance pack deletion has failed in the member account.</p> </li> <li> <p> <code>DELETE_IN_PROGRESS</code> when conformance pack is being deleted in the member account.</p> </li> <li> <p> <code>DELETE_SUCCESSFUL</code> when conformance pack has been deleted in the member account. </p> </li> <li> <p> <code>UPDATE_SUCCESSFUL</code> when conformance pack has been updated in the member account.</p> </li> <li> <p> <code>UPDATE_IN_PROGRESS</code> when conformance pack is being updated in the member account.</p> </li> <li> <p> <code>UPDATE_FAILED</code> when conformance pack deletion has failed in the member account.</p> </li> </ul>\"\n        }\n      ]\n\
  \    },\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"An error code that is returned when conformance pack creation or deletion failed in the member account. \"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"An error message indicating that conformance pack account creation or deletion has failed due to an error in the member account. \"\n        }\n      ]\n    },\n    \"LastUpdateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The timestamp of the last status update.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccountId\",\n    \"ConformancePackName\",\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-conformance-pack-detailed-status-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: OrganizationConformancePackDetailedStatus
---
