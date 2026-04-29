---
description: CollectInformation schema from Adyen API
layout: schema
name: CollectInformation
properties_list:
- description: Indicates whether [bank account details](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-checks/bank-account-check) must be collected. Default is **true**.
  name: bankDetails
  type: boolean
- description: Indicates whether [business details](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-checks/company-check) must be collected. Default is **true**.
  name: businessDetails
  type: boolean
- description: Indicates whether [individual details](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-checks/identity-check) must be collected. Default is **true**.
  name: individualDetails
  type: boolean
- description: Indicates whether [legal arrangement details](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-checks/legal-arrangements) must be collected. Default is **true**.
  name: legalArrangementDetails
  type: boolean
- description: Indicates whether answers to a [PCI questionnaire](https://docs.adyen.com/marketplaces-and-platforms/classic/platforms-for-partners#onboard-partner-platform) must be collected. Applies only to partner
  name: pciQuestionnaire
  type: boolean
- description: Indicates whether [shareholder details](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-checks/identity-check) must be collected. Defaults to **true**.
  name: shareholderDetails
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/hosted-onboarding-collect-information-schema.json
slug: hosted-onboarding-collect-information
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/hosted-onboarding-collect-information-schema.json\",\n  \"title\": \"CollectInformation\",\n  \"description\": \"CollectInformation schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bankDetails\": {\n      \"description\": \"Indicates whether [bank account details](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-checks/bank-account-check) must be collected. Default is **true**.\",\n      \"type\": \"boolean\"\n    },\n    \"businessDetails\": {\n      \"description\": \"Indicates whether [business details](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-checks/company-check) must be collected. Default is **true**.\",\n      \"type\": \"boolean\"\n    },\n    \"individualDetails\": {\n      \"description\": \"Indicates whether [individual details](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-checks/identity-check)\
  \ must be collected. Default is **true**.\",\n      \"type\": \"boolean\"\n    },\n    \"legalArrangementDetails\": {\n      \"description\": \"Indicates whether [legal arrangement details](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-checks/legal-arrangements) must be collected. Default is **true**.\",\n      \"type\": \"boolean\"\n    },\n    \"pciQuestionnaire\": {\n      \"description\": \"Indicates whether answers to a [PCI questionnaire](https://docs.adyen.com/marketplaces-and-platforms/classic/platforms-for-partners#onboard-partner-platform) must be collected. Applies only to partner platforms. Default is **true**.\",\n      \"type\": \"boolean\"\n    },\n    \"shareholderDetails\": {\n      \"description\": \"Indicates whether [shareholder details](https://docs.adyen.com/marketplaces-and-platforms/classic/verification-checks/identity-check) must be collected. Defaults to **true**.\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/hosted-onboarding-collect-information-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CollectInformation
---
