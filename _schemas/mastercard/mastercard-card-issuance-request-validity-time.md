---
description: Validity of the API request. It protects the API from unauthorized request or man-in-the-middle (MITM) attacks <br/>For example, if the validity of the API request is set for a maximum of 5 minutes (including retry attempts), and someone tries to post the same request after 5 minutes, then the system rejects the API request without processing.
layout: schema
name: RequestValidityTime
properties_list:
- description: The date and time after which the request is considered as invalid. If the timestamp of the institution is greater than this timestamp, the API request is considered as expired and is returned.<br/>Th
  name: dataValidUntilTimestamp
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-card-issuance-request-validity-time-schema.json
slug: mastercard-card-issuance-request-validity-time
source_filename: mastercard-card-issuance-request-validity-time-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RequestValidityTime\",\n  \"type\": \"object\",\n  \"description\": \"Validity of the API request. It protects the API from unauthorized request or man-in-the-middle (MITM) attacks <br/>For example, if the validity of the API request is set for a maximum of 5 minutes (including retry attempts), and someone tries to post the same request after 5 minutes, then the system rejects the API request without processing.\",\n  \"properties\": {\n    \"dataValidUntilTimestamp\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time after which the request is considered as invalid. If the timestamp of the institution is greater than this timestamp, the API request is considered as expired and is returned.<br/>The 'dataValidUntilTimestamp' parameter is converted into the institution time zone before comparing it with the institution date and time. It is expressed in ISO 8601 extended\
  \ format. Must be either <br/> 'YYYY-MM-DDThh:mm:ss[.sss]Z'<br/> or 'YYYY-MM-DDThh:mm:ss[.sss] (+|-) hh:mm' where [.sss] is optional and can be 1 to 3 digits.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-card-issuance-request-validity-time-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: RequestValidityTime
---
