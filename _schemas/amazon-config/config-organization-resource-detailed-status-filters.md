---
description: Status filter object to filter results based on specific member account ID or status type for an organization conformance pack.
layout: schema
name: OrganizationResourceDetailedStatusFilters
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-organization-resource-detailed-status-filters-schema.json
slug: config-organization-resource-detailed-status-filters
source_filename: config-organization-resource-detailed-status-filters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-resource-detailed-status-filters-schema.json\",\n  \"title\": \"OrganizationResourceDetailedStatusFilters\",\n  \"description\": \"Status filter object to filter results based on specific member account ID or status type for an organization conformance pack.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit account ID of the member account within an organization.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationResourceDetailedStatus\"\n        },\n        {\n          \"description\": \"<p>Indicates deployment status for conformance\
  \ pack in a member account. When management account calls <code>PutOrganizationConformancePack</code> action for the first time, conformance pack status is created in the member account. When management account calls <code>PutOrganizationConformancePack</code> action for the second time, conformance pack status is updated in the member account. Conformance pack status is deleted when the management account deletes <code>OrganizationConformancePack</code> and disables service access for <code>config-multiaccountsetup.amazonaws.com</code>. </p> <p> Config sets the state of the conformance pack to:</p> <ul> <li> <p> <code>CREATE_SUCCESSFUL</code> when conformance pack has been created in the member account. </p> </li> <li> <p> <code>CREATE_IN_PROGRESS</code> when conformance pack is being created in the member account.</p> </li> <li> <p> <code>CREATE_FAILED</code> when conformance pack creation has failed in the member account.</p> </li> <li> <p> <code>DELETE_FAILED</code> when conformance\
  \ pack deletion has failed in the member account.</p> </li> <li> <p> <code>DELETE_IN_PROGRESS</code> when conformance pack is being deleted in the member account.</p> </li> <li> <p> <code>DELETE_SUCCESSFUL</code> when conformance pack has been deleted in the member account. </p> </li> <li> <p> <code>UPDATE_SUCCESSFUL</code> when conformance pack has been updated in the member account.</p> </li> <li> <p> <code>UPDATE_IN_PROGRESS</code> when conformance pack is being updated in the member account.</p> </li> <li> <p> <code>UPDATE_FAILED</code> when conformance pack deletion has failed in the member account.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-resource-detailed-status-filters-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: OrganizationResourceDetailedStatusFilters
---
