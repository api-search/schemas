---
description: The DpaBatchStatus response contains information related to the status of a submitted Digital Payment Application (DPA) batch.
layout: schema
name: DpaBatchStatus
properties_list:
- description: This field allows the Integrator to assign an internal reference to a batch request so that it can be used for internal tracking purposes.
  name: requestId
  type: string
- description: A unique identifier associated with the submitted Digital Payment Application (DPA) batch. The Batch ID can be used to retrieve the status of the batch by calling GET DPA status endpoint.
  name: batchId
  type: string
- description: 'Describes the outcome of the submitted Digital Payment Application (DPA) batch. Possible outcomes include: * COMPLETED_SUCCESSFULLY - Batch was completed successfully and all DPAs included in the batc'
  name: batchStatus
  type: string
- description: Start time of batch request
  name: batchStartTime
  type: string
- description: End time of batch request
  name: batchEndTime
  type: string
- description: Provides additional information when batchStatus yields a FAILED status.
  name: errorMessage
  type: string
- description: 'An array of status objects that describes the outcome of each Digital Payment Application (DPA) item in a batch request. Note: DPA item order may differ from original submission."'
  name: items
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-checkout-solutions-dpa-batch-status-schema.json
slug: mastercard-checkout-solutions-dpa-batch-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DpaBatchStatus\",\n  \"type\": \"object\",\n  \"description\": \"The DpaBatchStatus response contains information related to the status of a submitted Digital Payment Application (DPA) batch.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"This field allows the Integrator to assign an internal reference to a batch request so that it can be used for internal tracking purposes.\"\n    },\n    \"batchId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier associated with the submitted Digital Payment Application (DPA) batch. The Batch ID can be used to retrieve the status of the batch by calling GET DPA status endpoint.\"\n    },\n    \"batchStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Describes the outcome of the submitted Digital Payment Application (DPA) batch. Possible outcomes include:\\n\\\
  n* COMPLETED_SUCCESSFULLY - Batch was completed successfully and all DPAs included in the batch are ready to transact.\\n\\n* COMPLETED_WITH_ERRORS - Batch was completed successfully, but some DPAs included in the batch aren't ready to transact.\\n\\n* FAILED -  Batch failed to load.\\n\\n* IN_PROGRESS - Batch processing in progress.\\n\\nFor a full breakdown of all DPA outcomes in a batch, refer to the items.\\n\"\n    },\n    \"batchStartTime\": {\n      \"type\": \"string\",\n      \"description\": \"Start time of batch request\"\n    },\n    \"batchEndTime\": {\n      \"type\": \"string\",\n      \"description\": \"End time of batch request\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Provides additional information when batchStatus yields a FAILED status.\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"An array of status objects that describes the outcome of each Digital Payment Application (DPA) item in\
  \ a batch request.\\n\\nNote: DPA item order may differ from original submission.\\\"\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-checkout-solutions-dpa-batch-status-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: DpaBatchStatus
---
