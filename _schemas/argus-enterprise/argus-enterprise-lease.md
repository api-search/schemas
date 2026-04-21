---
description: Represents a commercial real estate lease agreement in the ARGUS Enterprise platform, including tenant details, rent schedules, escalation terms, and lease options.
layout: schema
name: Argus Enterprise Lease
properties_list:
- description: Unique lease identifier
  name: id
  type: string
- description: Associated property identifier
  name: propertyId
  type: string
- description: Associated tenant identifier
  name: tenantId
  type: string
- description: Tenant name
  name: tenantName
  type: string
- description: Unit or suite number
  name: unitNumber
  type: string
- description: Type of lease
  name: leaseType
  type: string
- description: Current lease status
  name: status
  type: string
- description: Lease commencement date
  name: startDate
  type: string
- description: Lease expiration date
  name: endDate
  type: string
- description: Leased area in square feet
  name: leasedArea
  type: number
- description: Base rent amount per period
  name: baseRent
  type: number
- description: Rent payment frequency
  name: rentFrequency
  type: string
- description: Rent per square foot per annum
  name: rentPerSquareFoot
  type: number
- description: Annual rent escalation rate (percentage)
  name: escalationRate
  type: number
- description: Type of rent escalation
  name: escalationType
  type: string
- description: Security deposit amount
  name: securityDeposit
  type: number
- description: Tenant improvement allowance
  name: tenantImprovementAllowance
  type: number
- description: Lease renewal or expansion options
  name: options
  type: array
- description: Currency code (ISO 4217)
  name: currency
  type: string
- description: Record creation timestamp
  name: createdAt
  type: string
- description: Record last update timestamp
  name: updatedAt
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-lease-schema.json
slug: argus-enterprise-lease
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Argus Enterprise Lease
---
