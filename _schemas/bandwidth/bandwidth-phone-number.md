---
description: Represents a phone number managed through the Bandwidth Phone Numbers API, including its assignment, location metadata, and configured features.
layout: schema
name: Bandwidth Phone Number
properties_list:
- description: The full phone number, optionally in E.164 format
  name: fullNumber
  type: string
- description: The city associated with the phone number
  name: city
  type: string
- description: The two-letter state code associated with the phone number
  name: state
  type: string
- description: The Local Access and Transport Area (LATA) code
  name: lata
  type: string
- description: The rate center the phone number belongs to
  name: rateCenter
  type: string
- description: The current status of the phone number
  name: status
  type: string
- description: The site (sub-account) the number is assigned to
  name: siteId
  type: string
- description: The SIP peer (location) the number is assigned to
  name: sipPeerId
  type: string
- description: ''
  name: features
  type: object
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/bandwidth-phone-number-schema.json
slug: bandwidth-phone-number
source_filename: bandwidth-phone-number-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/bandwidth/phone-number.json\",\n  \"title\": \"Bandwidth Phone Number\",\n  \"description\": \"Represents a phone number managed through the Bandwidth Phone Numbers API, including its assignment, location metadata, and configured features.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fullNumber\": {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\+?1?[2-9]\\\\d{9}$\",\n      \"description\": \"The full phone number, optionally in E.164 format\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"The city associated with the phone number\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{2}$\",\n      \"description\": \"The two-letter state code associated with the phone number\"\n    },\n    \"lata\": {\n      \"type\": \"string\",\n      \"description\": \"The Local Access and\
  \ Transport Area (LATA) code\"\n    },\n    \"rateCenter\": {\n      \"type\": \"string\",\n      \"description\": \"The rate center the phone number belongs to\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Active\", \"Released\", \"PortOut\"],\n      \"description\": \"The current status of the phone number\"\n    },\n    \"siteId\": {\n      \"type\": \"string\",\n      \"description\": \"The site (sub-account) the number is assigned to\"\n    },\n    \"sipPeerId\": {\n      \"type\": \"string\",\n      \"description\": \"The SIP peer (location) the number is assigned to\"\n    },\n    \"features\": {\n      \"$ref\": \"#/$defs/NumberFeatures\"\n    }\n  },\n  \"$defs\": {\n    \"NumberFeatures\": {\n      \"type\": \"object\",\n      \"description\": \"Configured features for a phone number\",\n      \"properties\": {\n        \"callingNameDisplay\": {\n          \"type\": \"object\",\n          \"description\": \"CNAM (Caller Name) display configuration\"\
  ,\n          \"properties\": {\n            \"enabled\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether CNAM display is enabled\"\n            },\n            \"callingName\": {\n              \"type\": \"string\",\n              \"maxLength\": 15,\n              \"description\": \"The caller name to display (max 15 characters)\"\n            }\n          }\n        },\n        \"directoryListing\": {\n          \"type\": \"object\",\n          \"description\": \"Directory listing configuration\",\n          \"properties\": {\n            \"listed\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether the number is listed\"\n            },\n            \"listingType\": {\n              \"type\": \"string\",\n              \"enum\": [\"LISTED\", \"NON_LISTED\", \"NON_PUBLISHED\"],\n              \"description\": \"The type of directory listing\"\n            },\n            \"listingName\": {\n              \"type\": \"string\"\
  ,\n              \"description\": \"The name for the directory listing\"\n            }\n          }\n        }\n      }\n    },\n    \"Site\": {\n      \"type\": \"object\",\n      \"description\": \"A site (sub-account) within a Bandwidth account\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique site identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The site name\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A description of the site\"\n        },\n        \"address\": {\n          \"$ref\": \"#/$defs/Address\"\n        }\n      }\n    },\n    \"SipPeer\": {\n      \"type\": \"object\",\n      \"description\": \"A SIP peer (location) within a site\",\n      \"properties\": {\n        \"peerId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique SIP peer identifier\"\n    \
  \    },\n        \"peerName\": {\n          \"type\": \"string\",\n          \"description\": \"The SIP peer name\"\n        },\n        \"isDefaultPeer\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is the default peer for the site\"\n        }\n      }\n    },\n    \"Order\": {\n      \"type\": \"object\",\n      \"description\": \"A phone number order\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"orderId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique order identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"maxLength\": 50,\n          \"description\": \"The order name (max 50 characters)\"\n        },\n        \"orderStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\"RECEIVED\", \"PROCESSING\", \"COMPLETE\", \"PARTIAL\", \"FAILED\"],\n          \"description\": \"The current order status\"\n        },\n        \"orderCreateDate\": {\n\
  \          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the order was created\"\n        },\n        \"siteId\": {\n          \"type\": \"string\",\n          \"description\": \"The target site for ordered numbers\"\n        },\n        \"peerId\": {\n          \"type\": \"string\",\n          \"description\": \"The target SIP peer for ordered numbers\"\n        }\n      }\n    },\n    \"PortInRequest\": {\n      \"type\": \"object\",\n      \"description\": \"A phone number port-in request\",\n      \"properties\": {\n        \"portInId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique port-in request identifier\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The current port-in status\"\n        },\n        \"billingTelephoneNumber\": {\n          \"type\": \"string\",\n          \"description\": \"The billing telephone number for the porting account\"\n\
  \        },\n        \"losingCarrierName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the losing carrier\"\n        },\n        \"requestedFocDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"The requested Firm Order Commitment date\"\n        },\n        \"phoneNumbers\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"The phone numbers being ported\"\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"description\": \"A physical address\",\n      \"properties\": {\n        \"houseNumber\": {\n          \"type\": \"string\",\n          \"description\": \"The house or building number\"\n        },\n        \"streetName\": {\n          \"type\": \"string\",\n          \"description\": \"The street name\"\n        },\n        \"city\": {\n          \"type\": \"string\",\n      \
  \    \"description\": \"The city\"\n        },\n        \"stateCode\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\",\n          \"description\": \"The two-letter state code\"\n        },\n        \"zip\": {\n          \"type\": \"string\",\n          \"pattern\": \"^\\\\d{5}$\",\n          \"description\": \"The five-digit ZIP code\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"The country code\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/bandwidth-phone-number-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Bandwidth Phone Number
---
