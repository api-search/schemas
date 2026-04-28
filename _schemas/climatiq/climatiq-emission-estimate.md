---
description: Schema for the JSON object returned by Climatiq estimation endpoints. An emission estimate quantifies CO2-equivalent emissions for a single activity by combining a chosen emission factor with caller-supplied activity parameters such as energy used, distance travelled, money spent, or weight moved.
layout: schema
name: Climatiq Emission Estimate
properties_list:
- description: Total CO2-equivalent emissions for the activity, expressed in co2e_unit.
  name: co2e
  type: number
- description: Unit of measure for co2e (typically 'kg').
  name: co2e_unit
  type: string
- description: Calculation methodology used for the estimate (for example, ar4, ar5, ar6).
  name: co2e_calculation_method
  type: string
- description: Source of the calculation (for example, source for factors derived directly from a referenced source).
  name: co2e_calculation_origin
  type: string
- description: Metadata describing the emission factor used to produce this estimate.
  name: emission_factor
  type: object
- description: Breakdown of the estimate into constituent greenhouse gases.
  name: constituent_gases
  type: object
- description: Echo of the activity inputs used in the calculation.
  name: activity_data
  type: object
- description: Reference to the audit-trail entry recorded for this estimate when audit-trail is enabled.
  name: audit_trail
  type: string
provider_name: Climatiq
provider_slug: climatiq
schema_file: json-schema/climatiq-emission-estimate-schema.json
slug: climatiq-emission-estimate
tags:
- Carbon Accounting
- Carbon Emissions
- Climate
- Energy
- Environment
- GHG Protocol
- Sustainability
title: Climatiq Emission Estimate
---
