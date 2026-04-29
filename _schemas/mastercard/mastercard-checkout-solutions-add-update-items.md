---
description: ''
layout: schema
name: AddUpdateItems
properties_list:
- description: The action to be performed on the Digital Payment Application (DPA). The selected action will be applied to all DPAs provided in the items list. ADD - Add DPA UPDATE - Update DPA DELETE - Delete DPA N
  name: action
  type: string
- description: 'Conditional: The Customer Identifier (CID) must be passed when the Integrator is acting On-Behalf-Of (OBO) a client, registering through the Mastercard Connect (MC Connect) portal, or participating in'
  name: customerId
  type: string
- description: The Mastercard program that the Integrator would like to add their client(s) to. The Integrator must be enrolled in the program prior to enrolling their client(s). Integrators may view their active pr
  name: programType
  type: string
- description: The Token Requestor Identifier (TRID) should be passed by MDES for Merchants (M4M) Integrators who would like to onboard their M4M TRIDs to be used on Secure Card on File (SCOF).
  name: trid
  type: string
- description: A unique identifier assigned by Mastercard for which tokens are created uniquely for the entity onboarded.
  name: serviceId
  type: string
- description: Assign a category to the sub-merchant group identified in the request. For example, sub-merchants can be grouped by common attributes such as merchant category code (MCC), volume of transactions, or g
  name: category
  type: string
- description: 'The Cardholder facing name of the Merchant. Conditional: Must be supplied when adding Merchants to all Secure Card On File (SECURE_COF) programs.'
  name: programName
  type: string
- description: Dpas Object for Integrator to provide a list of Digital Processing Application (DPA) objects. Each DPA object is used to create a corresponding DPA. A minimum of 1 DPA object (to a maximum of 80 DPA o
  name: dpas
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-checkout-solutions-add-update-items-schema.json
slug: mastercard-checkout-solutions-add-update-items
source_filename: mastercard-checkout-solutions-add-update-items-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AddUpdateItems\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"The action to be performed on the Digital Payment Application (DPA). The selected action will be applied to all DPAs provided in the items list.\\n\\nADD - Add DPA\\n\\nUPDATE - Update DPA\\n\\nDELETE - Delete DPA\\n\\nNote:\\n* A limited number of DPA fields can be changed using the __UPDATE__ action. These are `dpaPresentationName`, `programName`, `dpaLogoUri`, `debitTokenRequested`, `merchantCategoryCode`, and `threeDSDefaultData`. Please refer to the example for a minimal use case.\\n* All DPA data from the original request (including non-updatable fields) will also need to be provided unchanged in the __PUT__ request for the operation to process successfully.\\n\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Conditional:\
  \ The Customer Identifier (CID) must be passed when the Integrator is acting On-Behalf-Of (OBO) a client, registering through the Mastercard Connect (MC Connect) portal, or participating in the Secure Card on File (SCOF) program.\\n\\nThis field should be populated with the CID of the Integrator's client (e.g., a Payment Service Provider (PSP) would pass the CID of the client they are integrating, i.e. DASP model).\\n\"\n    },\n    \"programType\": {\n      \"type\": \"string\",\n      \"description\": \"The Mastercard program that the Integrator would like to add their client(s) to. The Integrator must be enrolled in the program prior to enrolling their client(s). Integrators may view their active programs in the Mastercard Connect (MC Connect) portal.\\n\\n`SECURE_COF_MERCHANT` -  Integrating Merchant managing network tokenization. Tokens generated are unique for each merchant.\\n\\n`SECURE_COF_MERCHANT_OBO` - Integrating Payment Service Provider (PSP) managing network tokenization\
  \ for their Merchant(s). Tokens generated are unique for each merchant.\\n\\n`SECURE_COF_COMMERCE_PLATFORM` - Integrating Commerce Platform managing network tokenization. Tokens are generated unique for each Commerce Platform (tokens will be shared among their marketplace).\\n\\n`SECURE_COF_COMMERCE_PLATFORM_OBO` - Integrating PSPs managing network tokenization for their Commerce Platform(s). Tokens are generated unique for each Commerce Platform (tokens will be shared among their marketplace).\\n\\n`SECURE_COF_MERCHANT_OBO_SHARED` - Integrating PSPs managing network tokenization for their sub-Merchants. Tokens generated are unique for each Merchant Group.\\n\\n`SRC` - Integrating Merchants and PSPs participating in or offering the Click to Pay (C2P) program.\\n\\n`GUEST_CHECKOUT_TOKENIZATION` - A checkout solution that uses an alternative identifier to Account PANs, generated by the issuing network for guest checkout tokenization.\\n\\nNote: Other programTypes (e.g., AUTOFILL, SQR_DEVICE\
  \ etc.) may be available to select regions. Please contact your Mastercard representative for more details.\\n\"\n    },\n    \"trid\": {\n      \"type\": \"string\",\n      \"description\": \"The Token Requestor Identifier (TRID) should be passed by MDES for Merchants (M4M) Integrators who would like to onboard their M4M TRIDs to be used on Secure Card on File (SCOF).\"\n    },\n    \"serviceId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier assigned by Mastercard for which tokens are created uniquely for the entity onboarded.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Assign a category to the sub-merchant group identified in the request. For example, sub-merchants can be grouped by common attributes such as merchant category code (MCC), volume of transactions, or geography. Required for the SECURE_COF_MERCHANT_OBO_SHARED program type. Examples: \\\"discount stores\\\" and \\\"bakeries\\\"\"\n    },\n    \"programName\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The Cardholder facing name of the Merchant.\\n\\nConditional: Must be supplied when adding Merchants to all Secure Card On File (SECURE_COF) programs.\\n\"\n    },\n    \"dpas\": {\n      \"type\": \"array\",\n      \"description\": \"Dpas\\n\\nObject for Integrator to provide a list of Digital Processing Application (DPA) objects. Each DPA object is used to create a corresponding DPA. A minimum of 1 DPA object (to a maximum of 80 DPA objects) must be provided in the request.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-checkout-solutions-add-update-items-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: AddUpdateItems
---
