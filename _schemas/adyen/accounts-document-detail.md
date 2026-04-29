---
description: DocumentDetail schema from Adyen API
layout: schema
name: DocumentDetail
properties_list:
- description: The code of account holder, to which the document applies.
  name: accountHolderCode
  type: string
- description: The Adyen-generated [`bankAccountUUID`](https://docs.adyen.com/api-explorer/#/Account/latest/post/createAccountHolder__resParam_accountHolderDetails-bankAccountDetails-bankAccountUUID) to which the do
  name: bankAccountUUID
  type: string
- description: Description of the document.
  name: description
  type: string
- description: The type of the document. Refer to [Verification checks](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-checks) for details on when each document type should be submitted and f
  name: documentType
  type: string
- description: Filename of the document.
  name: filename
  type: string
- description: The Adyen-generated [`legalArrangementCode`](https://docs.adyen.com/api-explorer/#/Account/latest/post/createAccountHolder__resParam_accountHolderDetails-legalArrangements-legalArrangementCode) to whi
  name: legalArrangementCode
  type: string
- description: The Adyen-generated [`legalArrangementEntityCode`](https://docs.adyen.com/api-explorer/#/Account/v6/post/createAccountHolder__resParam_accountHolderDetails-legalArrangements-legalArrangementEntities-l
  name: legalArrangementEntityCode
  type: string
- description: The Adyen-generated [`shareholderCode`](https://docs.adyen.com/api-explorer/#/Account/latest/post/createAccountHolder__resParam_accountHolderDetails-businessDetails-shareholders-shareholderCode) to wh
  name: shareholderCode
  type: string
- description: The Adyen-generated [`signatoryCode`](https://docs.adyen.com/api-explorer/#/Account/v6/post/createAccountHolder__resParam_accountHolderDetails-businessDetails-signatories-signatoryCode) to which the d
  name: signatoryCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounts-document-detail-schema.json
slug: accounts-document-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-document-detail-schema.json\",\n  \"title\": \"DocumentDetail\",\n  \"description\": \"DocumentDetail schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderCode\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The code of account holder, to which the document applies.\",\n      \"type\": \"string\"\n    },\n    \"bankAccountUUID\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The Adyen-generated [`bankAccountUUID`](https://docs.adyen.com/api-explorer/#/Account/latest/post/createAccountHolder__resParam_accountHolderDetails-bankAccountDetails-bankAccountUUID) to which the document must be linked. Refer to [Bank account check](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-checks/bank-account-check#uploading-a-bank-statement)\
  \ for details on when a document should be submitted.\\n>Required if the `documentType` is **BANK_STATEMENT**, where a document is being submitted in order to verify a bank account.\\n\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"Description of the document.\",\n      \"type\": \"string\"\n    },\n    \"documentType\": {\n      \"description\": \"The type of the document. Refer to [Verification checks](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-checks) for details on when each document type should be submitted and for the accepted file formats.\\n\\nPermitted values:\\n* **BANK_STATEMENT**: A file containing a bank statement or other document proving ownership of a specific bank account.\\n* **COMPANY_REGISTRATION_SCREENING** (Supported from v5 and later): A file containing a company registration document.\\n* **CONSTITUTIONAL_DOCUMENT**: A file containing information about the account holder's legal arrangement.\\\
  n* **PASSPORT**: A file containing the identity page(s) of a passport.\\n* **ID_CARD_FRONT**: A file containing only the front of the ID card. In order for a document to be usable, both the **ID_CARD_FRONT** and **ID_CARD_BACK** must be submitted.\\n* **ID_CARD_BACK**: A file containing only the back of the ID card. In order for a document to be usable, both the **ID_CARD_FRONT** and **ID_CARD_BACK** must be submitted.\\n* **DRIVING_LICENCE_FRONT**: A file containing only the front of the driving licence. In order for a document to be usable, both the **DRIVING_LICENCE_FRONT** and **DRIVING_LICENCE_BACK** must be submitted.\\n* **DRIVING_LICENCE_BACK**: A file containing only the back of the driving licence. In order for a document to be usable, both the **DRIVING_LICENCE_FRONT** and **DRIVING_LICENCE_FRONT** must be submitted.\\n\",\n      \"enum\": [\n        \"BANK_STATEMENT\",\n        \"BSN\",\n        \"COMPANY_REGISTRATION_SCREENING\",\n        \"CONSTITUTIONAL_DOCUMENT\",\n   \
  \     \"DRIVING_LICENCE\",\n        \"DRIVING_LICENCE_BACK\",\n        \"DRIVING_LICENCE_FRONT\",\n        \"ID_CARD\",\n        \"ID_CARD_BACK\",\n        \"ID_CARD_FRONT\",\n        \"PASSPORT\",\n        \"PROOF_OF_RESIDENCY\",\n        \"SSN\",\n        \"SUPPORTING_DOCUMENTS\"\n      ],\n      \"type\": \"string\"\n    },\n    \"filename\": {\n      \"description\": \"Filename of the document.\",\n      \"type\": \"string\"\n    },\n    \"legalArrangementCode\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The Adyen-generated [`legalArrangementCode`](https://docs.adyen.com/api-explorer/#/Account/latest/post/createAccountHolder__resParam_accountHolderDetails-legalArrangements-legalArrangementCode) to which the document must be linked.\",\n      \"type\": \"string\"\n    },\n    \"legalArrangementEntityCode\": {\n      \"x-addedInVersion\": \"6\",\n      \"description\": \"The Adyen-generated [`legalArrangementEntityCode`](https://docs.adyen.com/api-explorer/#/Account/v6/post/createAccountHolder__resParam_accountHolderDetails-legalArrangements-legalArrangementEntities-legalArrangementEntityCode)\
  \  to which the document must be linked.\",\n      \"type\": \"string\"\n    },\n    \"shareholderCode\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The Adyen-generated [`shareholderCode`](https://docs.adyen.com/api-explorer/#/Account/latest/post/createAccountHolder__resParam_accountHolderDetails-businessDetails-shareholders-shareholderCode) to which the document must be linked. Refer to [Verification checks](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-checks) for details on when a document should be submitted.\\n>Required if the account holder has a `legalEntity` of type **Business** and the `documentType` is either **PASSPORT**, **ID_CARD_FRONT**, **ID_CARD_BACK**, **DRIVING_LICENCE_FRONT**, or **DRIVING_LICENCE_BACK**. \",\n      \"type\": \"string\"\n    },\n    \"signatoryCode\": {\n      \"description\": \"The Adyen-generated [`signatoryCode`](https://docs.adyen.com/api-explorer/#/Account/v6/post/createAccountHolder__resParam_accountHolderDetails-businessDetails-signatories-signatoryCode)\
  \ to which the document must be linked.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"documentType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounts-document-detail-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DocumentDetail
---
