---
description: Describes a maintenance action pending for an DMS resource, including when and how it will be applied. This data type is a response element to the <code>DescribePendingMaintenanceActions</code> operation.
layout: schema
name: PendingMaintenanceAction
properties_list:
- description: ''
  name: Action
  type: object
- description: ''
  name: AutoAppliedAfterDate
  type: object
- description: ''
  name: ForcedApplyDate
  type: object
- description: ''
  name: OptInStatus
  type: object
- description: ''
  name: CurrentApplyDate
  type: object
- description: ''
  name: Description
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-pending-maintenance-action-schema.json
slug: amazon-dms-pending-maintenance-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-pending-maintenance-action-schema.json\",\n  \"title\": \"PendingMaintenanceAction\",\n  \"description\": \"Describes a maintenance action pending for an DMS resource, including when and how it will be applied. This data type is a response element to the <code>DescribePendingMaintenanceActions</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type of pending maintenance action that is available for the resource.\"\n        }\n      ]\n    },\n    \"AutoAppliedAfterDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The date of the\
  \ maintenance window when the action is to be applied. The maintenance action is applied to the resource during its first maintenance window after this date. If this date is specified, any <code>next-maintenance</code> opt-in requests are ignored.\"\n        }\n      ]\n    },\n    \"ForcedApplyDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The date when the maintenance action will be automatically applied. The maintenance action is applied to the resource on this date regardless of the maintenance window for the resource. If this date is specified, any <code>immediate</code> opt-in requests are ignored.\"\n        }\n      ]\n    },\n    \"OptInStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type of opt-in request that has been received for the resource.\"\n        }\n      ]\n    },\n\
  \    \"CurrentApplyDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The effective date when the pending maintenance action will be applied to the resource. This date takes into account opt-in requests received from the <code>ApplyPendingMaintenanceAction</code> API operation, and also the <code>AutoAppliedAfterDate</code> and <code>ForcedApplyDate</code> parameter values. This value is blank if an opt-in request has not been received and nothing has been specified for <code>AutoAppliedAfterDate</code> or <code>ForcedApplyDate</code>.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A description providing more detail about the maintenance action.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-pending-maintenance-action-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: PendingMaintenanceAction
---
