---
description: IndividualDetails schema from Adyen API
layout: schema
name: IndividualDetails
properties_list:
- description: The name of the individual. >Make sure your account holder registers using the name shown on their Photo ID.
  name: name
  type: object
- description: Personal information of the individual.
  name: personalData
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-individual-details-schema.json
slug: notifications-individual-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-individual-details-schema.json\",\n  \"title\": \"IndividualDetails\",\n  \"description\": \"IndividualDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"The name of the individual.\\n>Make sure your account holder registers using the name shown on their Photo ID.\",\n      \"$ref\": \"#/components/schemas/ViasName\"\n    },\n    \"personalData\": {\n      \"description\": \"Personal information of the individual.\",\n      \"$ref\": \"#/components/schemas/ViasPersonalData\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-individual-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: IndividualDetails
---
