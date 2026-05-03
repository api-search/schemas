---
description: Schema for SAP S/4HANA Sales Order entity (A_SalesOrder) from the API_SALES_ORDER_SRV OData service. Represents a sales order header with organizational data, dates, pricing, and status information.
layout: schema
name: SAP Sales Order
properties_list:
- description: Sales order number
  name: SalesOrder
  type: string
- description: Sales document type (e.g., OR=Standard Order, RE=Return)
  name: SalesOrderType
  type: string
- description: Sales organization
  name: SalesOrganization
  type: string
- description: Distribution channel
  name: DistributionChannel
  type: string
- description: Division
  name: OrganizationDivision
  type: string
- description: Sales group
  name: SalesGroup
  type: string
- description: Sales office
  name: SalesOffice
  type: string
- description: Sales district
  name: SalesDistrict
  type: string
- description: Sold-to party customer number
  name: SoldToParty
  type: string
- description: Date on which the sales order was created
  name: CreationDate
  type: string
- description: User who created the sales order
  name: CreatedByUser
  type: string
- description: Date of last change
  name: LastChangeDate
  type: string
- description: UTC timestamp of last change
  name: LastChangeDateTime
  type: string
- description: Customer purchase order number
  name: PurchaseOrderByCustomer
  type: string
- description: Customer purchase order type
  name: CustomerPurchaseOrderType
  type: string
- description: Customer purchase order date
  name: CustomerPurchaseOrderDate
  type: string
- description: Document date of the sales order
  name: SalesOrderDate
  type: string
- description: Net value of the sales order in document currency
  name: TotalNetAmount
  type: string
- description: SD document currency (ISO 4217)
  name: TransactionCurrency
  type: string
- description: Order reason
  name: SDDocumentReason
  type: string
- description: Date for pricing and exchange rate determination
  name: PricingDate
  type: string
- description: Requested delivery date
  name: RequestedDeliveryDate
  type: string
- description: Shipping conditions
  name: ShippingCondition
  type: string
- description: Complete delivery flag
  name: CompleteDeliveryIsDefined
  type: boolean
- description: Billing block for the header
  name: HeaderBillingBlockReason
  type: string
- description: Delivery block for the header
  name: DeliveryBlockReason
  type: string
- description: Incoterms (part 1)
  name: IncotermsClassification
  type: string
- description: Incoterms (part 2)
  name: IncotermsTransferLocation
  type: string
- description: Payment method
  name: PaymentMethod
  type: string
- description: Terms of payment key
  name: CustomerPaymentTerms
  type: string
- description: Overall processing status (A=Not yet processed, B=Partially processed, C=Completely processed)
  name: OverallSDProcessStatus
  type: string
- description: Overall status of credit checks
  name: TotalCreditCheckStatus
  type: string
- description: Overall delivery status
  name: OverallDeliveryStatus
  type: string
- description: Overall billing status
  name: OverallBillingStatus
  type: string
provider_name: SAP Sales and Distribution (SD)
provider_slug: sap-sales-and-distribution-sd
schema_file: json-schema/sap-sd-sales-order-schema.json
slug: sap-sd-sales-order
source_filename: sap-sd-sales-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.sap.com/schemas/sap-sd-sales-order\",\n  \"title\": \"SAP Sales Order\",\n  \"description\": \"Schema for SAP S/4HANA Sales Order entity (A_SalesOrder) from the API_SALES_ORDER_SRV OData service. Represents a sales order header with organizational data, dates, pricing, and status information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SalesOrder\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Sales order number\"\n    },\n    \"SalesOrderType\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Sales document type (e.g., OR=Standard Order, RE=Return)\"\n    },\n    \"SalesOrganization\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Sales organization\"\n    },\n    \"DistributionChannel\": {\n      \"type\": \"string\",\n      \"maxLength\": 2,\n      \"description\"\
  : \"Distribution channel\"\n    },\n    \"OrganizationDivision\": {\n      \"type\": \"string\",\n      \"maxLength\": 2,\n      \"description\": \"Division\"\n    },\n    \"SalesGroup\": {\n      \"type\": \"string\",\n      \"maxLength\": 3,\n      \"description\": \"Sales group\"\n    },\n    \"SalesOffice\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Sales office\"\n    },\n    \"SalesDistrict\": {\n      \"type\": \"string\",\n      \"maxLength\": 6,\n      \"description\": \"Sales district\"\n    },\n    \"SoldToParty\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Sold-to party customer number\"\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date on which the sales order was created\"\n    },\n    \"CreatedByUser\": {\n      \"type\": \"string\",\n      \"maxLength\": 12,\n      \"description\": \"User who created the sales order\"\n\
  \    },\n    \"LastChangeDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of last change\"\n    },\n    \"LastChangeDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"UTC timestamp of last change\"\n    },\n    \"PurchaseOrderByCustomer\": {\n      \"type\": \"string\",\n      \"maxLength\": 35,\n      \"description\": \"Customer purchase order number\"\n    },\n    \"CustomerPurchaseOrderType\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Customer purchase order type\"\n    },\n    \"CustomerPurchaseOrderDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Customer purchase order date\"\n    },\n    \"SalesOrderDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Document date of the sales order\"\n    },\n    \"TotalNetAmount\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"Net value of the sales order in document currency\"\n    },\n    \"TransactionCurrency\": {\n      \"type\": \"string\",\n      \"maxLength\": 5,\n      \"description\": \"SD document currency (ISO 4217)\"\n    },\n    \"SDDocumentReason\": {\n      \"type\": \"string\",\n      \"maxLength\": 3,\n      \"description\": \"Order reason\"\n    },\n    \"PricingDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date for pricing and exchange rate determination\"\n    },\n    \"RequestedDeliveryDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Requested delivery date\"\n    },\n    \"ShippingCondition\": {\n      \"type\": \"string\",\n      \"maxLength\": 2,\n      \"description\": \"Shipping conditions\"\n    },\n    \"CompleteDeliveryIsDefined\": {\n      \"type\": \"boolean\",\n      \"description\": \"Complete delivery flag\"\n    },\n    \"HeaderBillingBlockReason\": {\n      \"\
  type\": \"string\",\n      \"maxLength\": 2,\n      \"description\": \"Billing block for the header\"\n    },\n    \"DeliveryBlockReason\": {\n      \"type\": \"string\",\n      \"maxLength\": 2,\n      \"description\": \"Delivery block for the header\"\n    },\n    \"IncotermsClassification\": {\n      \"type\": \"string\",\n      \"maxLength\": 3,\n      \"description\": \"Incoterms (part 1)\"\n    },\n    \"IncotermsTransferLocation\": {\n      \"type\": \"string\",\n      \"maxLength\": 28,\n      \"description\": \"Incoterms (part 2)\"\n    },\n    \"PaymentMethod\": {\n      \"type\": \"string\",\n      \"maxLength\": 1,\n      \"description\": \"Payment method\"\n    },\n    \"CustomerPaymentTerms\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Terms of payment key\"\n    },\n    \"OverallSDProcessStatus\": {\n      \"type\": \"string\",\n      \"maxLength\": 1,\n      \"description\": \"Overall processing status (A=Not yet processed, B=Partially\
  \ processed, C=Completely processed)\"\n    },\n    \"TotalCreditCheckStatus\": {\n      \"type\": \"string\",\n      \"maxLength\": 1,\n      \"description\": \"Overall status of credit checks\"\n    },\n    \"OverallDeliveryStatus\": {\n      \"type\": \"string\",\n      \"maxLength\": 1,\n      \"description\": \"Overall delivery status\"\n    },\n    \"OverallBillingStatus\": {\n      \"type\": \"string\",\n      \"maxLength\": 1,\n      \"description\": \"Overall billing status\"\n    }\n  },\n  \"required\": [\"SalesOrder\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/json-schema/sap-sd-sales-order-schema.json
tags:
- Distribution
- ERP
- OData
- S/4HANA
- Sales
- SAP
title: SAP Sales Order
---
