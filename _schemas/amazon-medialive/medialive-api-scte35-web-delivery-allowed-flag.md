---
description: Corresponds to the web_delivery_allowed_flag parameter. A value of WEB_DELIVERY_NOT_ALLOWED corresponds to 0 (false) in the SCTE-35 specification. If you include one of the "restriction" flags then you must include all four of them.
layout: schema
name: Scte35WebDeliveryAllowedFlag
properties_list: []
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-scte35-web-delivery-allowed-flag-schema.json
slug: medialive-api-scte35-web-delivery-allowed-flag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-web-delivery-allowed-flag-schema.json\",\n  \"title\": \"Scte35WebDeliveryAllowedFlag\",\n  \"description\": \"Corresponds to the web_delivery_allowed_flag parameter. A value of WEB_DELIVERY_NOT_ALLOWED corresponds to 0 (false) in the SCTE-35 specification. If you include one of the \\\"restriction\\\" flags then you must include all four of them.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"WEB_DELIVERY_NOT_ALLOWED\",\n    \"WEB_DELIVERY_ALLOWED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-web-delivery-allowed-flag-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Scte35WebDeliveryAllowedFlag
---
