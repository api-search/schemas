---
description: Sales order item entity (A_SalesOrderItem) representing a line item in a sales order. Contains material, quantity, pricing, plant assignment, and item-level processing status.
layout: schema
name: SalesOrderItem
properties_list:
- description: Sales order number the item belongs to
  name: SalesOrder
  type: string
- description: Sales order item number (e.g., '000010')
  name: SalesOrderItem
  type: string
- description: Higher-level item number in a BOM structure
  name: HigherLevelItem
  type: string
- description: Item category (e.g., TAN for standard item, TANN for free-of-charge)
  name: SalesOrderItemCategory
  type: string
- description: Short text description of the item
  name: SalesOrderItemText
  type: string
- description: Customer purchase order number at item level
  name: PurchaseOrderByCustomer
  type: string
- description: Material number
  name: Material
  type: string
- description: Material number used by the customer
  name: MaterialByCustomer
  type: string
- description: Pricing date at item level
  name: PricingDate
  type: string
- description: Billing plan number
  name: BillingPlan
  type: string
- description: Requested quantity
  name: RequestedQuantity
  type: string
- description: Unit of measure for the requested quantity (ISO unit code)
  name: RequestedQuantityUnit
  type: string
- description: SAP internal unit of measure
  name: RequestedQuantitySAPUnit
  type: string
- description: Indicator that the requested quantity is fixed
  name: RequestedQuantityIsFixed
  type: boolean
- description: Gross weight of the item
  name: ItemGrossWeight
  type: string
- description: Net weight of the item
  name: ItemNetWeight
  type: string
- description: Weight unit (e.g., KG, LB)
  name: ItemWeightUnit
  type: string
- description: Volume of the item
  name: ItemVolume
  type: string
- description: Volume unit
  name: ItemVolumeUnit
  type: string
- description: Transaction currency (ISO 4217)
  name: TransactionCurrency
  type: string
- description: Net value of the item in document currency
  name: NetAmount
  type: string
- description: Total SD amount
  name: TotalSDAmount
  type: string
- description: Material group
  name: MaterialGroup
  type: string
- description: Material pricing group
  name: MaterialPricingGroup
  type: string
- description: Batch number
  name: Batch
  type: string
- description: Production plant
  name: ProductionPlant
  type: string
- description: Storage location
  name: StorageLocation
  type: string
- description: Delivery group
  name: DeliveryGroup
  type: string
- description: Shipping point or receiving point
  name: ShippingPoint
  type: string
- description: Shipping type
  name: ShippingType
  type: string
- description: Delivery priority
  name: DeliveryPriority
  type: string
- description: Incoterms at item level
  name: IncotermsClassification
  type: string
- description: Incoterms location at item level
  name: IncotermsTransferLocation
  type: string
- description: Payment terms at item level
  name: CustomerPaymentTerms
  type: string
- description: Tax classification for material
  name: ProductTaxClassification1
  type: string
- description: Reason for rejection of the item
  name: SalesDocumentRjcnReason
  type: string
- description: Billing block at item level
  name: ItemBillingBlockReason
  type: string
- description: WBS element for project assignment
  name: WBSElement
  type: string
- description: Profit center
  name: ProfitCenter
  type: string
- description: Internal order number
  name: OrderID
  type: string
- description: Cost center
  name: CostCenter
  type: string
- description: Reference document number
  name: ReferenceSDDocument
  type: string
- description: Reference document item
  name: ReferenceSDDocumentItem
  type: string
- description: Processing status at item level
  name: SDProcessStatus
  type: string
- description: Delivery status
  name: DeliveryStatus
  type: string
- description: Order-related billing status
  name: OrderRelatedBillingStatus
  type: string
- description: Plant (delivering plant)
  name: Plant
  type: string
- description: Warehouse number
  name: WarehouseNumber
  type: string
- description: Customer group
  name: CustomerGroup
  type: string
- description: Sales district
  name: SalesDistrict
  type: string
- description: Item usage
  name: CustomerMaterialItemUsage
  type: string
- description: Navigation to item pricing elements
  name: to_PricingElement
  type: array
- description: Navigation to item schedule lines
  name: to_ScheduleLine
  type: array
- description: Navigation to item partner functions
  name: to_Partner
  type: array
- description: Navigation to item text records
  name: to_Text
  type: array
provider_name: SAP S/4HANA
provider_slug: sap-s4hana
schema_file: json-schema/sap-s4hana-sales-order-sales-order-item-schema.json
slug: sap-s4hana-sales-order-sales-order-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SalesOrderItem\",\n  \"type\": \"object\",\n  \"description\": \"Sales order item entity (A_SalesOrderItem) representing a line item in a sales order. Contains material, quantity, pricing, plant assignment, and item-level processing status.\",\n  \"properties\": {\n    \"SalesOrder\": {\n      \"type\": \"string\",\n      \"description\": \"Sales order number the item belongs to\"\n    },\n    \"SalesOrderItem\": {\n      \"type\": \"string\",\n      \"description\": \"Sales order item number (e.g., '000010')\"\n    },\n    \"HigherLevelItem\": {\n      \"type\": \"string\",\n      \"description\": \"Higher-level item number in a BOM structure\"\n    },\n    \"SalesOrderItemCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Item category (e.g., TAN for standard item, TANN for free-of-charge)\"\n    },\n    \"SalesOrderItemText\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Short text description of the item\"\n    },\n    \"PurchaseOrderByCustomer\": {\n      \"type\": \"string\",\n      \"description\": \"Customer purchase order number at item level\"\n    },\n    \"Material\": {\n      \"type\": \"string\",\n      \"description\": \"Material number\"\n    },\n    \"MaterialByCustomer\": {\n      \"type\": \"string\",\n      \"description\": \"Material number used by the customer\"\n    },\n    \"PricingDate\": {\n      \"type\": \"string\",\n      \"description\": \"Pricing date at item level\"\n    },\n    \"BillingPlan\": {\n      \"type\": \"string\",\n      \"description\": \"Billing plan number\"\n    },\n    \"RequestedQuantity\": {\n      \"type\": \"string\",\n      \"description\": \"Requested quantity\"\n    },\n    \"RequestedQuantityUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measure for the requested quantity (ISO unit code)\"\n    },\n    \"RequestedQuantitySAPUnit\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"SAP internal unit of measure\"\n    },\n    \"RequestedQuantityIsFixed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicator that the requested quantity is fixed\"\n    },\n    \"ItemGrossWeight\": {\n      \"type\": \"string\",\n      \"description\": \"Gross weight of the item\"\n    },\n    \"ItemNetWeight\": {\n      \"type\": \"string\",\n      \"description\": \"Net weight of the item\"\n    },\n    \"ItemWeightUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Weight unit (e.g., KG, LB)\"\n    },\n    \"ItemVolume\": {\n      \"type\": \"string\",\n      \"description\": \"Volume of the item\"\n    },\n    \"ItemVolumeUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Volume unit\"\n    },\n    \"TransactionCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction currency (ISO 4217)\"\n    },\n    \"NetAmount\": {\n      \"type\": \"string\",\n      \"description\": \"Net value of the item\
  \ in document currency\"\n    },\n    \"TotalSDAmount\": {\n      \"type\": \"string\",\n      \"description\": \"Total SD amount\"\n    },\n    \"MaterialGroup\": {\n      \"type\": \"string\",\n      \"description\": \"Material group\"\n    },\n    \"MaterialPricingGroup\": {\n      \"type\": \"string\",\n      \"description\": \"Material pricing group\"\n    },\n    \"Batch\": {\n      \"type\": \"string\",\n      \"description\": \"Batch number\"\n    },\n    \"ProductionPlant\": {\n      \"type\": \"string\",\n      \"description\": \"Production plant\"\n    },\n    \"StorageLocation\": {\n      \"type\": \"string\",\n      \"description\": \"Storage location\"\n    },\n    \"DeliveryGroup\": {\n      \"type\": \"string\",\n      \"description\": \"Delivery group\"\n    },\n    \"ShippingPoint\": {\n      \"type\": \"string\",\n      \"description\": \"Shipping point or receiving point\"\n    },\n    \"ShippingType\": {\n      \"type\": \"string\",\n      \"description\": \"Shipping\
  \ type\"\n    },\n    \"DeliveryPriority\": {\n      \"type\": \"string\",\n      \"description\": \"Delivery priority\"\n    },\n    \"IncotermsClassification\": {\n      \"type\": \"string\",\n      \"description\": \"Incoterms at item level\"\n    },\n    \"IncotermsTransferLocation\": {\n      \"type\": \"string\",\n      \"description\": \"Incoterms location at item level\"\n    },\n    \"CustomerPaymentTerms\": {\n      \"type\": \"string\",\n      \"description\": \"Payment terms at item level\"\n    },\n    \"ProductTaxClassification1\": {\n      \"type\": \"string\",\n      \"description\": \"Tax classification for material\"\n    },\n    \"SalesDocumentRjcnReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for rejection of the item\"\n    },\n    \"ItemBillingBlockReason\": {\n      \"type\": \"string\",\n      \"description\": \"Billing block at item level\"\n    },\n    \"WBSElement\": {\n      \"type\": \"string\",\n      \"description\": \"WBS element\
  \ for project assignment\"\n    },\n    \"ProfitCenter\": {\n      \"type\": \"string\",\n      \"description\": \"Profit center\"\n    },\n    \"OrderID\": {\n      \"type\": \"string\",\n      \"description\": \"Internal order number\"\n    },\n    \"CostCenter\": {\n      \"type\": \"string\",\n      \"description\": \"Cost center\"\n    },\n    \"ReferenceSDDocument\": {\n      \"type\": \"string\",\n      \"description\": \"Reference document number\"\n    },\n    \"ReferenceSDDocumentItem\": {\n      \"type\": \"string\",\n      \"description\": \"Reference document item\"\n    },\n    \"SDProcessStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Processing status at item level\"\n    },\n    \"DeliveryStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Delivery status\"\n    },\n    \"OrderRelatedBillingStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Order-related billing status\"\n    },\n    \"Plant\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Plant (delivering plant)\"\n    },\n    \"WarehouseNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Warehouse number\"\n    },\n    \"CustomerGroup\": {\n      \"type\": \"string\",\n      \"description\": \"Customer group\"\n    },\n    \"SalesDistrict\": {\n      \"type\": \"string\",\n      \"description\": \"Sales district\"\n    },\n    \"CustomerMaterialItemUsage\": {\n      \"type\": \"string\",\n      \"description\": \"Item usage\"\n    },\n    \"to_PricingElement\": {\n      \"type\": \"array\",\n      \"description\": \"Navigation to item pricing elements\"\n    },\n    \"to_ScheduleLine\": {\n      \"type\": \"array\",\n      \"description\": \"Navigation to item schedule lines\"\n    },\n    \"to_Partner\": {\n      \"type\": \"array\",\n      \"description\": \"Navigation to item partner functions\"\n    },\n    \"to_Text\": {\n      \"type\": \"array\",\n      \"description\": \"Navigation to item text records\"\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-s4hana/refs/heads/main/json-schema/sap-s4hana-sales-order-sales-order-item-schema.json
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
title: SalesOrderItem
---
