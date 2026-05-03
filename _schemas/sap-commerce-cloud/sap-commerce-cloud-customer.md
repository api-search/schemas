---
description: A customer account in SAP Commerce Cloud representing a registered user with profile information, addresses, payment methods, and consent preferences.
layout: schema
name: SAP Commerce Cloud Customer
properties_list:
- description: Unique user identifier, typically the email address
  name: uid
  type: string
- description: Internal customer identifier
  name: customerId
  type: string
- description: Full display name
  name: name
  type: string
- description: First name
  name: firstName
  type: string
- description: Last name
  name: lastName
  type: string
- description: Title code (e.g., mr, mrs, ms, dr)
  name: titleCode
  type: string
- description: Display UID (email or formatted identifier)
  name: displayUid
  type: string
- description: ''
  name: currency
  type: object
- description: ''
  name: language
  type: object
- description: ''
  name: defaultAddress
  type: object
- description: Customer address book
  name: addresses
  type: array
- description: Saved payment methods
  name: paymentDetails
  type: array
- description: Consent preferences
  name: consentTemplates
  type: array
provider_name: SAP Commerce Cloud
provider_slug: sap-commerce-cloud
schema_file: json-schema/sap-commerce-cloud-customer-schema.json
slug: sap-commerce-cloud-customer
source_filename: sap-commerce-cloud-customer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.sap.com/schemas/sap-commerce-cloud/customer.json\",\n  \"title\": \"SAP Commerce Cloud Customer\",\n  \"description\": \"A customer account in SAP Commerce Cloud representing a registered user with profile information, addresses, payment methods, and consent preferences.\",\n  \"type\": \"object\",\n  \"required\": [\"uid\"],\n  \"properties\": {\n    \"uid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique user identifier, typically the email address\",\n      \"minLength\": 1\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Internal customer identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full display name\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Last name\"\n    },\n    \"titleCode\": {\n      \"type\": \"string\",\n      \"description\": \"Title code (e.g., mr, mrs, ms, dr)\"\n    },\n    \"displayUid\": {\n      \"type\": \"string\",\n      \"description\": \"Display UID (email or formatted identifier)\"\n    },\n    \"currency\": {\n      \"$ref\": \"#/$defs/Currency\"\n    },\n    \"language\": {\n      \"$ref\": \"#/$defs/Language\"\n    },\n    \"defaultAddress\": {\n      \"$ref\": \"#/$defs/Address\"\n    },\n    \"addresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Address\"\n      },\n      \"description\": \"Customer address book\"\n    },\n    \"paymentDetails\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PaymentDetails\"\n      },\n      \"description\": \"Saved payment methods\"\n    },\n    \"consentTemplates\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ConsentTemplate\"\n      },\n      \"description\"\
  : \"Consent preferences\"\n    }\n  },\n  \"$defs\": {\n    \"Currency\": {\n      \"type\": \"object\",\n      \"description\": \"Preferred currency\",\n      \"properties\": {\n        \"isocode\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{3}$\",\n          \"description\": \"ISO 4217 currency code\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Currency display name\"\n        },\n        \"symbol\": {\n          \"type\": \"string\",\n          \"description\": \"Currency symbol\"\n        }\n      }\n    },\n    \"Language\": {\n      \"type\": \"object\",\n      \"description\": \"Preferred language\",\n      \"properties\": {\n        \"isocode\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 639-1 language code\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Language display name\"\n        }\n      }\n    },\n    \"Address\": {\n\
  \      \"type\": \"object\",\n      \"description\": \"Customer address\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Address identifier\"\n        },\n        \"firstName\": {\n          \"type\": \"string\",\n          \"description\": \"First name\"\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"description\": \"Last name\"\n        },\n        \"titleCode\": {\n          \"type\": \"string\",\n          \"description\": \"Title code\"\n        },\n        \"companyName\": {\n          \"type\": \"string\",\n          \"description\": \"Company name (B2B)\"\n        },\n        \"line1\": {\n          \"type\": \"string\",\n          \"description\": \"Address line 1\"\n        },\n        \"line2\": {\n          \"type\": \"string\",\n          \"description\": \"Address line 2\"\n        },\n        \"town\": {\n          \"type\": \"string\",\n          \"description\": \"City or town\"\
  \n        },\n        \"district\": {\n          \"type\": \"string\",\n          \"description\": \"District\"\n        },\n        \"region\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"isocode\": {\n              \"type\": \"string\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"postalCode\": {\n          \"type\": \"string\",\n          \"description\": \"Postal or ZIP code\"\n        },\n        \"country\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"isocode\": {\n              \"type\": \"string\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"phone\": {\n          \"type\": \"string\",\n          \"description\": \"Phone number\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\"\
  : \"Email address\"\n        },\n        \"defaultAddress\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is the default address\"\n        },\n        \"shippingAddress\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is a shipping address\"\n        },\n        \"billingAddress\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is a billing address\"\n        }\n      }\n    },\n    \"PaymentDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Saved payment method\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Payment details identifier\"\n        },\n        \"accountHolderName\": {\n          \"type\": \"string\",\n          \"description\": \"Card holder name\"\n        },\n        \"cardNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Masked card number\"\n        },\n        \"cardType\"\
  : {\n          \"type\": \"object\",\n          \"properties\": {\n            \"code\": {\n              \"type\": \"string\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"expiryMonth\": {\n          \"type\": \"string\",\n          \"description\": \"Expiry month (01-12)\"\n        },\n        \"expiryYear\": {\n          \"type\": \"string\",\n          \"description\": \"Expiry year (4-digit)\"\n        },\n        \"billingAddress\": {\n          \"$ref\": \"#/$defs/Address\"\n        },\n        \"defaultPayment\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this is the default payment method\"\n        },\n        \"saved\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the payment method is saved for future use\"\n        }\n      }\n    },\n    \"ConsentTemplate\": {\n      \"type\": \"object\",\n      \"description\": \"Consent template and\
  \ status\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Consent template identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Consent template name\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Consent description\"\n        },\n        \"version\": {\n          \"type\": \"integer\",\n          \"description\": \"Template version number\"\n        },\n        \"currentConsent\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"consentGivenDate\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\",\n              \"description\": \"When consent was given\"\n            },\n            \"consentWithdrawnDate\": {\n              \"type\": [\"string\", \"null\"],\n              \"format\": \"date-time\",\n              \"description\": \"When consent was withdrawn,\
  \ if applicable\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-commerce-cloud/refs/heads/main/json-schema/sap-commerce-cloud-customer-schema.json
tags:
- B2B
- B2C
- Commerce
- Customer Experience
- Ecommerce
- Omnichannel
- Retail
title: SAP Commerce Cloud Customer
---
