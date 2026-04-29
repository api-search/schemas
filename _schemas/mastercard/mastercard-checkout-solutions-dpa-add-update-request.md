---
description: 'The DpaAddUpdateRequest is used to add, update, or delete DPAs from the Mastercard system. Additionally, the DpaAddUpdateRequest can be used to generate serviceIds in Commerce Platform use cases. A Digital Payment Application (DPA) is a website, web or mobile application operated by a Merchant, marketplace, or other service provider where a consumer can purchase goods or services. A ServiceId is a unique identifier assigned by Mastercard for which tokens are created uniquely for the entity onboarded. A serviceId can have multiple associated DPAs. The DpaAddUpdateRequest request must contain the following values: * items * action * programType The contents of the DPA items will vary based on the operation requested.'
layout: schema
name: DpaAddUpdateRequest
properties_list:
- description: This field allows the Integrator to assign an internal reference to a batch request so that it can be used for internal tracking purposes.
  name: requestId
  type: string
- description: Items Object for Integrator to provide a list of Digital Payment Applications (DPA) to be enrolled in a given program. A minimum of 1 item must be provided in a request.
  name: items
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-checkout-solutions-dpa-add-update-request-schema.json
slug: mastercard-checkout-solutions-dpa-add-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DpaAddUpdateRequest\",\n  \"type\": \"object\",\n  \"description\": \"The DpaAddUpdateRequest is used to add, update, or delete DPAs from the Mastercard system. Additionally, the DpaAddUpdateRequest can be used to generate serviceIds in Commerce Platform use cases.\\n\\nA Digital Payment Application (DPA) is a website, web or mobile application operated by a Merchant, marketplace, or other service provider where a consumer can purchase goods or services.\\n\\nA ServiceId is a unique identifier assigned by Mastercard for which tokens are created uniquely for the entity onboarded. A serviceId can have multiple associated DPAs.\\n\\nThe DpaAddUpdateRequest request must contain the following values:\\n\\n * items\\n * action\\n * programType\\n\\n The contents of the DPA items will vary based on the operation requested.\\n\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"This field allows the Integrator to assign an internal reference to a batch request so that it can be used for internal tracking purposes.\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Items\\n\\nObject for Integrator to provide a list of Digital Payment Applications (DPA) to be enrolled in a given program. A minimum of 1 item must be provided in a request.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-checkout-solutions-dpa-add-update-request-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: DpaAddUpdateRequest
---
