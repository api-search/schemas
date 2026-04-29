---
description: DataCenter schema from Adyen API
layout: schema
name: DataCenter
properties_list:
- description: 'The unique [live URL prefix](https://docs.adyen.com/development-resources/live-endpoints#live-url-prefix) for your live endpoint. Each data center has its own live URL prefix. This field is empty for '
  name: livePrefix
  type: string
- description: 'The name assigned to a data center, for example **EU** for the European data center. Possible values are: * **default**: the European data center. This value is always returned in the test environment'
  name: name
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-data-center-schema.json
slug: management-data-center
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-data-center-schema.json\",\n  \"title\": \"DataCenter\",\n  \"description\": \"DataCenter schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"livePrefix\": {\n      \"description\": \"The unique [live URL prefix](https://docs.adyen.com/development-resources/live-endpoints#live-url-prefix) for your live endpoint. Each data center has its own live URL prefix.\\n\\nThis field is empty for requests made in the test environment.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name assigned to a data center, for example **EU** for the European data center. Possible values are:\\n\\n* **default**: the European data center. This value is always returned in the test environment. \\n* **AU**\\n* **EU**\\n* **US**\",\n      \"type\": \"string\"\n  \
  \  }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-data-center-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DataCenter
---
