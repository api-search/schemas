---
description: Represents a payment dispute filed by a customer against an Affirm transaction. Disputes are managed via the Affirm Disputes API V3, which supports listing disputes, submitting merchant evidence, and closing disputes. Merchants can contest disputes by uploading supporting documentation via the Files API.
layout: schema
name: Affirm Dispute
properties_list:
- description: Unique identifier for this dispute, assigned by Affirm.
  name: id
  type: string
- description: The identifier of the Affirm transaction being disputed.
  name: transaction_id
  type: string
- description: The identifier of the charge associated with this dispute.
  name: charge_id
  type: string
- description: Current lifecycle status of the dispute.
  name: status
  type: string
- description: Standardized reason code categorizing the nature of the customer's dispute claim.
  name: reason_code
  type: string
- description: The disputed amount in the smallest currency unit (e.g., cents for USD).
  name: amount
  type: integer
- description: The ISO 4217 currency code for the disputed amount.
  name: currency
  type: string
- description: Timestamp when this dispute was opened, in RFC 3339 format.
  name: created
  type: string
- description: Deadline by which the merchant must submit evidence to contest this dispute, in RFC 3339 format.
  name: evidence_due_by
  type: string
- description: Timestamp when this dispute was closed, if applicable. Null if still open.
  name: closed_at
  type:
  - string
  - 'null'
- description: Final resolution outcome after dispute review. Only set when status is won or lost.
  name: outcome
  type:
  - string
  - 'null'
- description: List of evidence items submitted by the merchant in response to this dispute.
  name: evidence
  type: array
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/affirm-dispute-schema.json
slug: affirm-dispute
source_filename: affirm-dispute-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://affirm.com/schemas/affirm/dispute.json\",\n  \"title\": \"Affirm Dispute\",\n  \"description\": \"Represents a payment dispute filed by a customer against an Affirm transaction. Disputes are managed via the Affirm Disputes API V3, which supports listing disputes, submitting merchant evidence, and closing disputes. Merchants can contest disputes by uploading supporting documentation via the Files API.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"status\", \"amount\", \"currency\", \"created\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this dispute, assigned by Affirm.\"\n    },\n    \"transaction_id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the Affirm transaction being disputed.\"\n    },\n    \"charge_id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier\
  \ of the charge associated with this dispute.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle status of the dispute.\",\n      \"enum\": [\"open\", \"closed\", \"won\", \"lost\"]\n    },\n    \"reason_code\": {\n      \"type\": \"string\",\n      \"description\": \"Standardized reason code categorizing the nature of the customer's dispute claim.\",\n      \"examples\": [\"item_not_received\", \"item_not_as_described\", \"unauthorized\", \"duplicate\", \"credit_not_processed\"]\n    },\n    \"amount\": {\n      \"type\": \"integer\",\n      \"description\": \"The disputed amount in the smallest currency unit (e.g., cents for USD).\",\n      \"minimum\": 0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 4217 currency code for the disputed amount.\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Timestamp when this dispute was opened, in RFC 3339 format.\"\n    },\n    \"evidence_due_by\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Deadline by which the merchant must submit evidence to contest this dispute, in RFC 3339 format.\"\n    },\n    \"closed_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when this dispute was closed, if applicable. Null if still open.\"\n    },\n    \"outcome\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Final resolution outcome after dispute review. Only set when status is won or lost.\",\n      \"enum\": [\"merchant_won\", \"merchant_lost\", null]\n    },\n    \"evidence\": {\n      \"type\": \"array\",\n      \"description\": \"List of evidence items submitted by the merchant in response to this dispute.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/EvidenceItem\"\n      }\n    }\n  },\n  \"$defs\"\
  : {\n    \"EvidenceItem\": {\n      \"type\": \"object\",\n      \"description\": \"A single piece of evidence submitted by the merchant to contest a dispute.\",\n      \"required\": [\"id\", \"type\", \"submitted_at\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for this evidence item.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The category of evidence represented by this item.\",\n          \"enum\": [\"file\", \"text\", \"tracking\"]\n        },\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"The evidence content. For file evidence, this is the file identifier from the Files API. For text evidence, this is the explanatory text.\"\n        },\n        \"submitted_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when this evidence was submitted,\
  \ in RFC 3339 format.\"\n        }\n      }\n    },\n    \"EvidenceRequest\": {\n      \"type\": \"object\",\n      \"description\": \"Request body for submitting evidence to contest a dispute via the Disputes API.\",\n      \"properties\": {\n        \"files\": {\n          \"type\": \"array\",\n          \"description\": \"Array of file identifiers from the Files API to attach as documentary evidence.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"explanation\": {\n          \"type\": \"string\",\n          \"description\": \"Textual explanation of the merchant's position supporting why the dispute should be decided in the merchant's favor.\",\n          \"maxLength\": 5000\n        },\n        \"tracking_number\": {\n          \"type\": \"string\",\n          \"description\": \"Shipment tracking number demonstrating the order was delivered as expected.\",\n          \"maxLength\": 200\n        },\n        \"shipping_carrier\": {\n  \
  \        \"type\": \"string\",\n          \"description\": \"Name of the shipping carrier used for the disputed order.\",\n          \"maxLength\": 200\n        },\n        \"customer_communication\": {\n          \"type\": \"string\",\n          \"description\": \"Description or summary of merchant communications with the customer regarding the disputed order.\",\n          \"maxLength\": 5000\n        },\n        \"refund_policy_disclosure\": {\n          \"type\": \"string\",\n          \"description\": \"The merchant's refund policy as presented to the customer at time of purchase.\",\n          \"maxLength\": 5000\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/affirm-dispute-schema.json
tags: []
title: Affirm Dispute
---
