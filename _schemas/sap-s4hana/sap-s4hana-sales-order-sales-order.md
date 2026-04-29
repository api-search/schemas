---
description: Sales order header entity (A_SalesOrder) representing a complete sales document in SAP S/4HANA. Contains organizational data, customer references, pricing totals, and processing status information.
layout: schema
name: SalesOrder
properties_list:
- description: Sales order number
  name: SalesOrder
  type: string
- description: Sales document type (e.g., OR for standard order, RE for returns)
  name: SalesOrderType
  type: string
- description: Sales organization responsible for the sales order
  name: SalesOrganization
  type: string
- description: Distribution channel through which the product reaches the customer
  name: DistributionChannel
  type: string
- description: Division for the sales organization
  name: OrganizationDivision
  type: string
- description: Sales group within the sales organization
  name: SalesGroup
  type: string
- description: Sales office responsible for the order
  name: SalesOffice
  type: string
- description: Geographic sales district
  name: SalesDistrict
  type: string
- description: Customer number of the sold-to party
  name: SoldToParty
  type: string
- description: Date when the sales order was created
  name: CreationDate
  type: string
- description: User who created the sales order
  name: CreatedByUser
  type: string
- description: Date of the last change to the sales order
  name: LastChangeDate
  type: string
- description: Timestamp of the last change including time zone
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
- description: Total net value of the sales order in document currency
  name: TotalNetAmount
  type: string
- description: Currency key for the sales order (ISO 4217)
  name: TransactionCurrency
  type: string
- description: Order reason (e.g., reason for return or credit memo)
  name: SDDocumentReason
  type: string
- description: Date used for pricing determination
  name: PricingDate
  type: string
- description: Requested delivery date for the entire order
  name: RequestedDeliveryDate
  type: string
- description: Shipping condition code
  name: ShippingCondition
  type: string
- description: Indicator for complete delivery requirement
  name: CompleteDeliveryIsDefined
  type: boolean
- description: Shipping type code
  name: ShippingType
  type: string
- description: Billing block reason at header level
  name: HeaderBillingBlockReason
  type: string
- description: Delivery block reason
  name: DeliveryBlockReason
  type: string
- description: Incoterms classification (e.g., FOB, CIF, EXW)
  name: IncotermsClassification
  type: string
- description: Incoterms location (named place)
  name: IncotermsTransferLocation
  type: string
- description: Incoterms location 1
  name: IncotermsLocation1
  type: string
- description: Incoterms location 2
  name: IncotermsLocation2
  type: string
- description: Incoterms version year
  name: IncotermsVersion
  type: string
- description: Payment terms key
  name: CustomerPaymentTerms
  type: string
- description: Payment method code
  name: PaymentMethod
  type: string
- description: Assignment reference number
  name: AssignmentReference
  type: string
- description: Reference document number (e.g., quotation or contract number)
  name: ReferenceSDDocument
  type: string
- description: Reference document category
  name: ReferenceSDDocumentCategory
  type: string
- description: Exchange rate for accounting
  name: AccountingExchangeRate
  type: string
- description: Overall processing status of the sales document (A=Not yet processed, B=Partially processed, C=Completely processed)
  name: OverallSDProcessStatus
  type: string
- description: Overall status of credit checks
  name: TotalCreditCheckStatus
  type: string
- description: Overall delivery status
  name: OverallTotalDeliveryStatus
  type: string
- description: Overall rejection status of the sales document
  name: OverallSDDocumentRejectionSts
  type: string
- description: Billing date for the entire order
  name: BillingDocumentDate
  type: string
- description: Contract account number
  name: ContractAccount
  type: string
- description: Customer group 1
  name: AdditionalCustomerGroup1
  type: string
- description: Customer group 2
  name: AdditionalCustomerGroup2
  type: string
- description: Customer group 3
  name: AdditionalCustomerGroup3
  type: string
- description: Customer group 4
  name: AdditionalCustomerGroup4
  type: string
- description: Customer group 5
  name: AdditionalCustomerGroup5
  type: string
- description: Indicator that the document is relevant for proof of delivery
  name: SlsDocIsRlvtForProofOfDeliv
  type: boolean
- description: Tax classification 1 for customer
  name: CustomerTaxClassification1
  type: string
- description: Tax classification 2 for customer
  name: CustomerTaxClassification2
  type: string
- description: Tax classification 3 for customer
  name: CustomerTaxClassification3
  type: string
- description: Tax classification 4 for customer
  name: CustomerTaxClassification4
  type: string
- description: Customer account group
  name: CustomerAccountGroup
  type: string
- description: Navigation to sales order items
  name: to_Item
  type: array
- description: Navigation to header partner functions
  name: to_Partner
  type: array
- description: Navigation to header pricing elements
  name: to_PricingElement
  type: array
- description: Navigation to header text records
  name: to_Text
  type: array
provider_name: SAP S/4HANA
provider_slug: sap-s4hana
schema_file: json-schema/sap-s4hana-sales-order-sales-order-schema.json
slug: sap-s4hana-sales-order-sales-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SalesOrder\",\n  \"type\": \"object\",\n  \"description\": \"Sales order header entity (A_SalesOrder) representing a complete sales document in SAP S/4HANA. Contains organizational data, customer references, pricing totals, and processing status information.\",\n  \"properties\": {\n    \"SalesOrder\": {\n      \"type\": \"string\",\n      \"description\": \"Sales order number\"\n    },\n    \"SalesOrderType\": {\n      \"type\": \"string\",\n      \"description\": \"Sales document type (e.g., OR for standard order, RE for returns)\"\n    },\n    \"SalesOrganization\": {\n      \"type\": \"string\",\n      \"description\": \"Sales organization responsible for the sales order\"\n    },\n    \"DistributionChannel\": {\n      \"type\": \"string\",\n      \"description\": \"Distribution channel through which the product reaches the customer\"\n    },\n    \"OrganizationDivision\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Division for the sales organization\"\n    },\n    \"SalesGroup\": {\n      \"type\": \"string\",\n      \"description\": \"Sales group within the sales organization\"\n    },\n    \"SalesOffice\": {\n      \"type\": \"string\",\n      \"description\": \"Sales office responsible for the order\"\n    },\n    \"SalesDistrict\": {\n      \"type\": \"string\",\n      \"description\": \"Geographic sales district\"\n    },\n    \"SoldToParty\": {\n      \"type\": \"string\",\n      \"description\": \"Customer number of the sold-to party\"\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date when the sales order was created\"\n    },\n    \"CreatedByUser\": {\n      \"type\": \"string\",\n      \"description\": \"User who created the sales order\"\n    },\n    \"LastChangeDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of the last change to the sales order\"\n    },\n    \"LastChangeDateTime\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of the last change including time zone\"\n    },\n    \"PurchaseOrderByCustomer\": {\n      \"type\": \"string\",\n      \"description\": \"Customer purchase order number\"\n    },\n    \"CustomerPurchaseOrderType\": {\n      \"type\": \"string\",\n      \"description\": \"Customer purchase order type\"\n    },\n    \"CustomerPurchaseOrderDate\": {\n      \"type\": \"string\",\n      \"description\": \"Customer purchase order date\"\n    },\n    \"SalesOrderDate\": {\n      \"type\": \"string\",\n      \"description\": \"Document date of the sales order\"\n    },\n    \"TotalNetAmount\": {\n      \"type\": \"string\",\n      \"description\": \"Total net value of the sales order in document currency\"\n    },\n    \"TransactionCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency key for the sales order (ISO 4217)\"\n    },\n    \"SDDocumentReason\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Order reason (e.g., reason for return or credit memo)\"\n    },\n    \"PricingDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date used for pricing determination\"\n    },\n    \"RequestedDeliveryDate\": {\n      \"type\": \"string\",\n      \"description\": \"Requested delivery date for the entire order\"\n    },\n    \"ShippingCondition\": {\n      \"type\": \"string\",\n      \"description\": \"Shipping condition code\"\n    },\n    \"CompleteDeliveryIsDefined\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicator for complete delivery requirement\"\n    },\n    \"ShippingType\": {\n      \"type\": \"string\",\n      \"description\": \"Shipping type code\"\n    },\n    \"HeaderBillingBlockReason\": {\n      \"type\": \"string\",\n      \"description\": \"Billing block reason at header level\"\n    },\n    \"DeliveryBlockReason\": {\n      \"type\": \"string\",\n      \"description\": \"Delivery block reason\"\n    },\n    \"IncotermsClassification\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Incoterms classification (e.g., FOB, CIF, EXW)\"\n    },\n    \"IncotermsTransferLocation\": {\n      \"type\": \"string\",\n      \"description\": \"Incoterms location (named place)\"\n    },\n    \"IncotermsLocation1\": {\n      \"type\": \"string\",\n      \"description\": \"Incoterms location 1\"\n    },\n    \"IncotermsLocation2\": {\n      \"type\": \"string\",\n      \"description\": \"Incoterms location 2\"\n    },\n    \"IncotermsVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Incoterms version year\"\n    },\n    \"CustomerPaymentTerms\": {\n      \"type\": \"string\",\n      \"description\": \"Payment terms key\"\n    },\n    \"PaymentMethod\": {\n      \"type\": \"string\",\n      \"description\": \"Payment method code\"\n    },\n    \"AssignmentReference\": {\n      \"type\": \"string\",\n      \"description\": \"Assignment reference number\"\n    },\n    \"ReferenceSDDocument\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Reference document number (e.g., quotation or contract number)\"\n    },\n    \"ReferenceSDDocumentCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Reference document category\"\n    },\n    \"AccountingExchangeRate\": {\n      \"type\": \"string\",\n      \"description\": \"Exchange rate for accounting\"\n    },\n    \"OverallSDProcessStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Overall processing status of the sales document (A=Not yet processed, B=Partially processed, C=Completely processed)\"\n    },\n    \"TotalCreditCheckStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Overall status of credit checks\"\n    },\n    \"OverallTotalDeliveryStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Overall delivery status\"\n    },\n    \"OverallSDDocumentRejectionSts\": {\n      \"type\": \"string\",\n      \"description\": \"Overall rejection status of the sales document\"\n\
  \    },\n    \"BillingDocumentDate\": {\n      \"type\": \"string\",\n      \"description\": \"Billing date for the entire order\"\n    },\n    \"ContractAccount\": {\n      \"type\": \"string\",\n      \"description\": \"Contract account number\"\n    },\n    \"AdditionalCustomerGroup1\": {\n      \"type\": \"string\",\n      \"description\": \"Customer group 1\"\n    },\n    \"AdditionalCustomerGroup2\": {\n      \"type\": \"string\",\n      \"description\": \"Customer group 2\"\n    },\n    \"AdditionalCustomerGroup3\": {\n      \"type\": \"string\",\n      \"description\": \"Customer group 3\"\n    },\n    \"AdditionalCustomerGroup4\": {\n      \"type\": \"string\",\n      \"description\": \"Customer group 4\"\n    },\n    \"AdditionalCustomerGroup5\": {\n      \"type\": \"string\",\n      \"description\": \"Customer group 5\"\n    },\n    \"SlsDocIsRlvtForProofOfDeliv\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicator that the document is relevant for proof of\
  \ delivery\"\n    },\n    \"CustomerTaxClassification1\": {\n      \"type\": \"string\",\n      \"description\": \"Tax classification 1 for customer\"\n    },\n    \"CustomerTaxClassification2\": {\n      \"type\": \"string\",\n      \"description\": \"Tax classification 2 for customer\"\n    },\n    \"CustomerTaxClassification3\": {\n      \"type\": \"string\",\n      \"description\": \"Tax classification 3 for customer\"\n    },\n    \"CustomerTaxClassification4\": {\n      \"type\": \"string\",\n      \"description\": \"Tax classification 4 for customer\"\n    },\n    \"CustomerAccountGroup\": {\n      \"type\": \"string\",\n      \"description\": \"Customer account group\"\n    },\n    \"to_Item\": {\n      \"type\": \"array\",\n      \"description\": \"Navigation to sales order items\"\n    },\n    \"to_Partner\": {\n      \"type\": \"array\",\n      \"description\": \"Navigation to header partner functions\"\n    },\n    \"to_PricingElement\": {\n      \"type\": \"array\",\n    \
  \  \"description\": \"Navigation to header pricing elements\"\n    },\n    \"to_Text\": {\n      \"type\": \"array\",\n      \"description\": \"Navigation to header text records\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/json-schema/sap-s4hana-sales-order-sales-order-schema.json
tags:
- Business Applications
- Cloud
- Enterprise Resource Planning
- ERP
- Finance
- Human Resources
- Inventory
- Logistics
- Manufacturing
- Plant Maintenance
- Procurement
- S/4HANA
- Sales
- SAP
title: SalesOrder
---
