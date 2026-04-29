---
description: This setting allows the delivery restriction flags on SCTE-35 segmentation descriptors to determine whether a message signals an ad. Choosing "NONE" means no SCTE-35 messages become ads. Choosing "RESTRICTED" means SCTE-35 messages of the types specified in AdTriggers that contain delivery restrictions will be treated as ads. Choosing "UNRESTRICTED" means SCTE-35 messages of the types specified in AdTriggers that do not contain delivery restrictions will be treated as ads. Choosing "BOTH" means all SCTE-35 messages of the types specified in AdTriggers will be treated as ads. Note that Splice Insert messages do not have these flags and are always treated as ads if specified in AdTriggers.
layout: schema
name: AdsOnDeliveryRestrictions
properties_list: []
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-ads-on-delivery-restrictions-schema.json
slug: mediapackage-api-ads-on-delivery-restrictions
source_filename: mediapackage-api-ads-on-delivery-restrictions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-ads-on-delivery-restrictions-schema.json\",\n  \"title\": \"AdsOnDeliveryRestrictions\",\n  \"description\": \"This setting allows the delivery restriction flags on SCTE-35 segmentation descriptors to\\ndetermine whether a message signals an ad.  Choosing \\\"NONE\\\" means no SCTE-35 messages become\\nads.  Choosing \\\"RESTRICTED\\\" means SCTE-35 messages of the types specified in AdTriggers that\\ncontain delivery restrictions will be treated as ads.  Choosing \\\"UNRESTRICTED\\\" means SCTE-35\\nmessages of the types specified in AdTriggers that do not contain delivery restrictions will\\nbe treated as ads.  Choosing \\\"BOTH\\\" means all SCTE-35 messages of the types specified in\\nAdTriggers will be treated as ads.  Note that Splice Insert messages do not have these flags\\\
  nand are always treated as ads if specified in AdTriggers.\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"NONE\",\n    \"RESTRICTED\",\n    \"UNRESTRICTED\",\n    \"BOTH\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-ads-on-delivery-restrictions-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AdsOnDeliveryRestrictions
---
