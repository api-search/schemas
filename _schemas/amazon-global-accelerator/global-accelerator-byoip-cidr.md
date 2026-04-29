---
description: <p>Information about an IP address range that is provisioned for use with your Amazon Web Services resources through bring your own IP address (BYOIP).</p> <p>The following describes each BYOIP <code>State</code> that your IP address range can be in.</p> <ul> <li> <p> <b>PENDING_PROVISIONING</b> — You’ve submitted a request to provision an IP address range but it is not yet provisioned with Global Accelerator.</p> </li> <li> <p> <b>READY</b> — The address range is provisioned with Global Accelerator and can be advertised.</p> </li> <li> <p> <b>PENDING_ADVERTISING</b> — You’ve submitted a request for Global Accelerator to advertise an address range but it is not yet being advertised.</p> </li> <li> <p> <b>ADVERTISING</b> — The address range is being advertised by Global Accelerator.</p> </li> <li> <p> <b>PENDING_WITHDRAWING</b> — You’ve submitted a request to withdraw an address range from being advertised but it is still being advertised by Global Accelerator.</p> </li> <li>
  <p> <b>PENDING_DEPROVISIONING</b> — You’ve submitted a request to deprovision an address range from Global Accelerator but it is still provisioned.</p> </li> <li> <p> <b>DEPROVISIONED</b> — The address range is deprovisioned from Global Accelerator.</p> </li> <li> <p> <b>FAILED_PROVISION </b> — The request to provision the address range from Global Accelerator was not successful. Please make sure that you provide all of the correct information, and try again. If the request fails a second time, contact Amazon Web Services support.</p> </li> <li> <p> <b>FAILED_ADVERTISING</b> — The request for Global Accelerator to advertise the address range was not successful. Please make sure that you provide all of the correct information, and try again. If the request fails a second time, contact Amazon Web Services support.</p> </li> <li> <p> <b>FAILED_WITHDRAW</b> — The request to withdraw the address range from advertising by Global Accelerator was not successful. Please make sure that you provide
  all of the correct information, and try again. If the request fails a second time, contact Amazon Web Services support.</p> </li> <li> <p> <b>FAILED_DEPROVISION </b> — The request to deprovision the address range from Global Accelerator was not successful. Please make sure that you provide all of the correct information, and try again. If the request fails a second time, contact Amazon Web Services support.</p> </li> </ul>
layout: schema
name: ByoipCidr
properties_list:
- description: ''
  name: Cidr
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: Events
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-byoip-cidr-schema.json
slug: global-accelerator-byoip-cidr
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-byoip-cidr-schema.json\",\n  \"title\": \"ByoipCidr\",\n  \"description\": \"<p>Information about an IP address range that is provisioned for use with your Amazon Web Services resources through bring your own IP address (BYOIP).</p> <p>The following describes each BYOIP <code>State</code> that your IP address range can be in.</p> <ul> <li> <p> <b>PENDING_PROVISIONING</b> \\u2014 You\\u2019ve submitted a request to provision an IP address range but it is not yet provisioned with Global Accelerator.</p> </li> <li> <p> <b>READY</b> \\u2014 The address range is provisioned with Global Accelerator and can be advertised.</p> </li> <li> <p> <b>PENDING_ADVERTISING</b> \\u2014 You\\u2019ve submitted a request for Global Accelerator to advertise an address range but it is not yet being\
  \ advertised.</p> </li> <li> <p> <b>ADVERTISING</b> \\u2014 The address range is being advertised by Global Accelerator.</p> </li> <li> <p> <b>PENDING_WITHDRAWING</b> \\u2014 You\\u2019ve submitted a request to withdraw an address range from being advertised but it is still being advertised by Global Accelerator.</p> </li> <li> <p> <b>PENDING_DEPROVISIONING</b> \\u2014 You\\u2019ve submitted a request to deprovision an address range from Global Accelerator but it is still provisioned.</p> </li> <li> <p> <b>DEPROVISIONED</b> \\u2014 The address range is deprovisioned from Global Accelerator.</p> </li> <li> <p> <b>FAILED_PROVISION </b> \\u2014 The request to provision the address range from Global Accelerator was not successful. Please make sure that you provide all of the correct information, and try again. If the request fails a second time, contact Amazon Web Services support.</p> </li> <li> <p> <b>FAILED_ADVERTISING</b> \\u2014 The request for Global Accelerator to advertise the address\
  \ range was not successful. Please make sure that you provide all of the correct information, and try again. If the request fails a second time, contact Amazon Web Services support.</p> </li> <li> <p> <b>FAILED_WITHDRAW</b> \\u2014 The request to withdraw the address range from advertising by Global Accelerator was not successful. Please make sure that you provide all of the correct information, and try again. If the request fails a second time, contact Amazon Web Services support.</p> </li> <li> <p> <b>FAILED_DEPROVISION </b> \\u2014 The request to deprovision the address range from Global Accelerator was not successful. Please make sure that you provide all of the correct information, and try again. If the request fails a second time, contact Amazon Web Services support.</p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Cidr\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\"\
  : \"The address range, in CIDR notation.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ByoipCidrState\"\n        },\n        {\n          \"description\": \"The state of the address pool.\"\n        }\n      ]\n    },\n    \"Events\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ByoipCidrEvents\"\n        },\n        {\n          \"description\": \"A history of status changes for an IP address range that you bring to Global Accelerator through bring your own IP address (BYOIP).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-byoip-cidr-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: ByoipCidr
---
