---
description: A job's shipping information, including inbound and outbound tracking numbers and shipping speed options.
layout: schema
name: ShippingDetails
properties_list:
- description: ''
  name: ShippingOption
  type: object
- description: ''
  name: InboundShipment
  type: object
- description: ''
  name: OutboundShipment
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-shipping-details-schema.json
slug: amazon-snow-family-shipping-details
source_filename: amazon-snow-family-shipping-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-shipping-details-schema.json\",\n  \"title\": \"ShippingDetails\",\n  \"description\": \"A job's shipping information, including inbound and outbound tracking numbers and shipping speed options.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ShippingOption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShippingOption\"\n        },\n        {\n          \"description\": \"<p>The shipping speed for a particular job. This speed doesn't dictate how soon you'll get the Snow device from the job's creation date. This speed represents how quickly it moves to its destination while in transit. Regional shipping speeds are as follows:</p> <ul> <li> <p>In Australia, you have access to express shipping. Typically, Snow devices shipped express are delivered\
  \ in about a day.</p> </li> <li> <p>In the European Union (EU), you have access to express shipping. Typically, Snow devices shipped express are delivered in about a day. In addition, most countries in the EU have access to standard shipping, which typically takes less than a week, one way.</p> </li> <li> <p>In India, Snow devices are delivered in one to seven days.</p> </li> <li> <p>In the United States of America (US), you have access to one-day shipping and two-day shipping.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"InboundShipment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Shipment\"\n        },\n        {\n          \"description\": \"The <code>Status</code> and <code>TrackingNumber</code> values for a Snow device being returned to Amazon Web Services for a particular job.\"\n        }\n      ]\n    },\n    \"OutboundShipment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Shipment\"\n        },\n    \
  \    {\n          \"description\": \"The <code>Status</code> and <code>TrackingNumber</code> values for a Snow device being delivered to the address that you specified for a particular job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-shipping-details-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: ShippingDetails
---
