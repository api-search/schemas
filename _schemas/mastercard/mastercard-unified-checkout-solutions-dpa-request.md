---
description: ''
layout: schema
name: DpaRequest
properties_list:
- description: Dpas Object for Integrator to provide a list of Digital Processing Application (DPA) objects. Each DPA object is used to create a corresponding DPA. A minimum of 1 DPA object must be provided in the r
  name: dpas
  type: array
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-unified-checkout-solutions-dpa-request-schema.json
slug: mastercard-unified-checkout-solutions-dpa-request
source_filename: mastercard-unified-checkout-solutions-dpa-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DpaRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dpas\": {\n      \"type\": \"array\",\n      \"description\": \"Dpas\\n\\nObject for Integrator to provide a list of Digital Processing Application (DPA) objects. Each DPA object is used to create a corresponding DPA. A minimum of 1 DPA object must be provided in the request.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-unified-checkout-solutions-dpa-request-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: DpaRequest
---
