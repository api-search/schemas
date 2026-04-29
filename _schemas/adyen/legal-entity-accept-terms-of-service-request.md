---
description: AcceptTermsOfServiceRequest schema from Adyen API
layout: schema
name: AcceptTermsOfServiceRequest
properties_list:
- description: The legal entity ID of the user accepting the Terms of Service. For organizations, this must be the individual legal entity ID of an authorized signatory for the organization. For sole proprietorships
  name: acceptedBy
  type: string
- description: The IP address of the user accepting the Terms of Service.
  name: ipAddress
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-accept-terms-of-service-request-schema.json
slug: legal-entity-accept-terms-of-service-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-accept-terms-of-service-request-schema.json\",\n  \"title\": \"AcceptTermsOfServiceRequest\",\n  \"description\": \"AcceptTermsOfServiceRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"acceptedBy\": {\n      \"description\": \"The legal entity ID of the user accepting the Terms of Service.\\n\\nFor organizations, this must be the individual legal entity ID of an authorized signatory for the organization.\\n\\nFor sole proprietorships, this must be the individual legal entity ID of the owner.\",\n      \"type\": \"string\"\n    },\n    \"ipAddress\": {\n      \"description\": \"The IP address of the user accepting the Terms of Service.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"acceptedBy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-accept-terms-of-service-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AcceptTermsOfServiceRequest
---
