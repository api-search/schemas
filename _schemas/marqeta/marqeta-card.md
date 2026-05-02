---
description: A Marqeta payment card resource. Cards are derived from card products and represent individual physical or virtual payment instruments issued to a cardholder. Each card belongs to a card product that defines its behavior, network affiliation, spending controls, and fulfillment options. Cards have a lifecycle managed through card transitions (UNACTIVATED -> ACTIVE -> SUSPENDED | TERMINATED).
layout: schema
name: Marqeta Card
properties_list:
- description: Unique identifier for the card on the Marqeta platform.
  name: token
  type: string
- description: Token of the card product this card was derived from. The card product controls the card's behavior and spending controls.
  name: card_product_token
  type: string
- description: Token of the cardholder (user) who owns this card.
  name: user_token
  type: string
- description: Token of the business account holder who owns this card, if applicable.
  name: business_token
  type: string
- description: Last four digits of the card's primary account number (PAN).
  name: last_four
  type: string
- description: Full 16-digit primary account number. Only returned at card creation when show_pan=true is specified.
  name: pan
  type: string
- description: Card verification value (CVV2). Only returned at card creation when show_cvv_number=true is specified.
  name: cvv_number
  type: string
- description: Card expiration date in MMYY format.
  name: expiration
  type: string
- description: ISO 8601 timestamp representing the exact card expiration date and time.
  name: expiration_time
  type: string
- description: Current state in the card lifecycle.
  name: state
  type: string
- description: Human-readable reason for the current card state.
  name: state_reason
  type: string
- description: Current fulfillment status for physical cards tracking production and delivery progress.
  name: fulfillment_status
  type: string
- description: ''
  name: fulfillment
  type: object
- description: Whether a PIN has been set for this card.
  name: pin_is_set
  type: boolean
- description: Control token for PIN translation, if applicable.
  name: translate_pin_from_control_token
  type: string
- description: Physical form factor of the card.
  name: instrument_type
  type: string
- description: Whether expedited fulfillment was requested for this physical card.
  name: expedite
  type: boolean
- description: Key-value pairs of custom metadata associated with this card. Maximum 20 pairs.
  name: metadata
  type: object
- description: ISO 8601 timestamp when the card was created.
  name: created_time
  type: string
- description: ISO 8601 timestamp when the card record was last modified.
  name: last_modified_time
  type: string
provider_name: marqeta
provider_slug: marqeta
schema_file: json-schema/marqeta-card-schema.json
slug: marqeta-card
source_filename: marqeta-card-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://marqeta.com/schemas/card.json\",\n  \"title\": \"Marqeta Card\",\n  \"description\": \"A Marqeta payment card resource. Cards are derived from card products and represent individual physical or virtual payment instruments issued to a cardholder. Each card belongs to a card product that defines its behavior, network affiliation, spending controls, and fulfillment options. Cards have a lifecycle managed through card transitions (UNACTIVATED -> ACTIVE -> SUSPENDED | TERMINATED).\",\n  \"type\": \"object\",\n  \"required\": [\"token\", \"card_product_token\", \"user_token\", \"state\", \"created_time\"],\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the card on the Marqeta platform.\",\n      \"maxLength\": 36\n    },\n    \"card_product_token\": {\n      \"type\": \"string\",\n      \"description\": \"Token of the card\
  \ product this card was derived from. The card product controls the card's behavior and spending controls.\",\n      \"maxLength\": 36\n    },\n    \"user_token\": {\n      \"type\": \"string\",\n      \"description\": \"Token of the cardholder (user) who owns this card.\",\n      \"maxLength\": 36\n    },\n    \"business_token\": {\n      \"type\": \"string\",\n      \"description\": \"Token of the business account holder who owns this card, if applicable.\",\n      \"maxLength\": 36\n    },\n    \"last_four\": {\n      \"type\": \"string\",\n      \"description\": \"Last four digits of the card's primary account number (PAN).\",\n      \"pattern\": \"^\\\\d{4}$\"\n    },\n    \"pan\": {\n      \"type\": \"string\",\n      \"description\": \"Full 16-digit primary account number. Only returned at card creation when show_pan=true is specified.\",\n      \"pattern\": \"^\\\\d{16}$\"\n    },\n    \"cvv_number\": {\n      \"type\": \"string\",\n      \"description\": \"Card verification value\
  \ (CVV2). Only returned at card creation when show_cvv_number=true is specified.\",\n      \"pattern\": \"^\\\\d{3}$\"\n    },\n    \"expiration\": {\n      \"type\": \"string\",\n      \"description\": \"Card expiration date in MMYY format.\",\n      \"pattern\": \"^\\\\d{4}$\"\n    },\n    \"expiration_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp representing the exact card expiration date and time.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current state in the card lifecycle.\",\n      \"enum\": [\"ACTIVE\", \"SUSPENDED\", \"TERMINATED\", \"UNACTIVATED\", \"LIMITED\", \"UNSUPPORTED\"]\n    },\n    \"state_reason\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable reason for the current card state.\",\n      \"maxLength\": 255\n    },\n    \"fulfillment_status\": {\n      \"type\": \"string\",\n      \"description\": \"Current fulfillment status for\
  \ physical cards tracking production and delivery progress.\",\n      \"enum\": [\"ISSUED\", \"ORDERED\", \"REORDERED\", \"REJECTED\", \"SHIPPED\", \"DELIVERED\", \"DIGITALLY_PRESENTED\"]\n    },\n    \"fulfillment\": {\n      \"$ref\": \"#/$defs/CardFulfillment\"\n    },\n    \"pin_is_set\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether a PIN has been set for this card.\"\n    },\n    \"translate_pin_from_control_token\": {\n      \"type\": \"string\",\n      \"description\": \"Control token for PIN translation, if applicable.\"\n    },\n    \"instrument_type\": {\n      \"type\": \"string\",\n      \"description\": \"Physical form factor of the card.\",\n      \"enum\": [\"PHYSICAL_MSR\", \"PHYSICAL_ICC\", \"PHYSICAL_CONTACTLESS\", \"PHYSICAL_COMBO\", \"VIRTUAL_PAN\"]\n    },\n    \"expedite\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether expedited fulfillment was requested for this physical card.\"\n    },\n    \"metadata\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"Key-value pairs of custom metadata associated with this card. Maximum 20 pairs.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"maxProperties\": 20\n    },\n    \"created_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the card was created.\"\n    },\n    \"last_modified_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the card record was last modified.\"\n    }\n  },\n  \"$defs\": {\n    \"CardFulfillment\": {\n      \"type\": \"object\",\n      \"description\": \"Fulfillment configuration and shipping details for a physical card.\",\n      \"properties\": {\n        \"shipping\": {\n          \"$ref\": \"#/$defs/CardShipping\"\n        },\n        \"card_personalization\": {\n          \"$ref\": \"#/$defs/CardPersonalization\"\n        }\n      }\n    },\n   \
  \ \"CardShipping\": {\n      \"type\": \"object\",\n      \"description\": \"Shipping method and address for physical card delivery.\",\n      \"properties\": {\n        \"method\": {\n          \"type\": \"string\",\n          \"description\": \"Shipping service level for card delivery.\",\n          \"enum\": [\"LOCAL_MAIL\", \"GROUND\", \"TWO_DAY\", \"OVERNIGHT\", \"INTERNATIONAL\"]\n        },\n        \"return_address\": {\n          \"$ref\": \"#/$defs/ShippingAddress\"\n        },\n        \"recipient_address\": {\n          \"$ref\": \"#/$defs/ShippingAddress\"\n        },\n        \"care_of_line\": {\n          \"type\": \"string\",\n          \"description\": \"Care-of line printed on the card envelope.\",\n          \"maxLength\": 40\n        }\n      }\n    },\n    \"ShippingAddress\": {\n      \"type\": \"object\",\n      \"description\": \"Physical mailing address for card shipping.\",\n      \"required\": [\"first_name\", \"last_name\", \"address1\", \"city\", \"state\"\
  , \"zip\", \"country\"],\n      \"properties\": {\n        \"first_name\": {\n          \"type\": \"string\",\n          \"description\": \"First name of the recipient.\",\n          \"maxLength\": 40\n        },\n        \"middle_name\": {\n          \"type\": \"string\",\n          \"description\": \"Middle name of the recipient.\",\n          \"maxLength\": 40\n        },\n        \"last_name\": {\n          \"type\": \"string\",\n          \"description\": \"Last name of the recipient.\",\n          \"maxLength\": 40\n        },\n        \"address1\": {\n          \"type\": \"string\",\n          \"description\": \"Primary street address.\",\n          \"maxLength\": 255\n        },\n        \"address2\": {\n          \"type\": \"string\",\n          \"description\": \"Secondary address line.\",\n          \"maxLength\": 255\n        },\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City.\",\n          \"maxLength\": 40\n        },\n        \"state\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"State or province (two-letter abbreviation for US).\",\n          \"maxLength\": 32\n        },\n        \"zip\": {\n          \"type\": \"string\",\n          \"description\": \"ZIP or postal code.\",\n          \"maxLength\": 10\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"Two-letter ISO 3166-1 alpha-2 country code.\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"description\": \"Recipient's phone number.\"\n        }\n      }\n    },\n    \"CardPersonalization\": {\n      \"type\": \"object\",\n      \"description\": \"Custom personalization details printed on the physical card.\",\n      \"properties\": {\n        \"text\": {\n          \"type\": \"object\",\n          \"description\": \"Text printed on the card face.\",\n          \"properties\": {\n            \"name_line_1\": {\n       \
  \       \"type\": \"object\",\n              \"description\": \"First name line on the card.\",\n              \"properties\": {\n                \"value\": {\n                  \"type\": \"string\",\n                  \"description\": \"Text to print on name line 1.\",\n                  \"maxLength\": 26\n                }\n              }\n            },\n            \"name_line_2\": {\n              \"type\": \"object\",\n              \"description\": \"Second name line on the card.\",\n              \"properties\": {\n                \"value\": {\n                  \"type\": \"string\",\n                  \"description\": \"Text to print on name line 2.\",\n                  \"maxLength\": 26\n                }\n              }\n            }\n          }\n        },\n        \"images\": {\n          \"type\": \"object\",\n          \"description\": \"Custom images to print on the card.\",\n          \"properties\": {\n            \"card\": {\n              \"type\": \"object\",\n\
  \              \"description\": \"Custom card image configuration.\",\n              \"properties\": {\n                \"name\": {\n                  \"type\": \"string\",\n                  \"description\": \"Name of the card image design.\"\n                },\n                \"thermal_color\": {\n                  \"type\": \"string\",\n                  \"description\": \"Color scheme for thermal printing.\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/marqeta/refs/heads/main/json-schema/marqeta-card-schema.json
tags: []
title: Marqeta Card
---
