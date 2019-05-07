# ![LOGO](logo.png) Transportation Laws and Incentives **flow**ground Connector

## Description

A generated **flow**ground connector for the Transportation Laws and Incentives API (version 0.1.0).

Generated from: https://api.apis.guru/v2/specs/nrel.gov/transportation-incentives-laws/0.1.0/swagger.json<br/>
Generated at: 2019-05-07T17:43:18+03:00

## API Description

Query our database of State and Federal Laws and Incentives for Alternative Fuels

## Authorization

Supported authorization schemes:
- API Key
## Actions

### Return a full list of laws and incentives that match your query.

*Tags:* `v1`

#### Input Parameters
* `output_format` - _required_ - Response format
    Possible values: json, xml, csv.
* `limit` - _optional_ - Limit the number of laws returned
* `jurisdiction` - _optional_ - Return laws for the given Jurisdiction. Jurisdiction must be given as a two character state code (eg, 'CO' for Colorado). A single jurisdiction, or a comma-separate list of multiple jurisdiction, may be given.  Use the code 'US' for federal laws and the code 'DC' for Washington D.C.
* `technology` - _optional_ - Search by the technology type. A single type, or a comma-separate list of multiple types, may be given. Values and what they stand for are as follows: 'BIOD' for Biodiesel, 'ETH' for Ethanol, 'NG' for Natural Gas, 'LPG' for Propane (LPG), 'HY' for Hydrogen Fuel Cells, 'EFFEC' for Fuel Economy / Efficiency, 'IR' for Idle Reduction, 'ELEC' for EVs, 'HEV' for HEVs, 'PHEV' for PHEVs, 'OTHER' for Other, 'AFTMKTCONV' for Aftermarket Conversions, and 'NEVS' for NEVs
* `incentive_type` - _optional_ - Search by the incentive type. A single type, or a comma-separate list of multiple types, may be given. Values and what they stand for are as follows: 'GNT' for Grants, 'TAX' for Tax Incentives, 'LOANS' for Loans and Leases, 'RBATE' for Rebates, 'EXEM' for Exemptions, and 'OTHER' for Other.
* `regulation_type` - _optional_ - Search by the regulation type. A single type, or a comma-separate list of multiple types, may be given. Values and what they stand for are as follows: 'REGIS' for Registration / Licensing, 'STD' for Fuel Production / Quality, 'DREST' for Driving / Idling, 'REQ' for Acquisition / Fuel Use, 'FUEL' for Fuel Taxes, 'RFS' for Renewable Fuel Standard / Mandate, 'OTHER' for Other, 'AIRQEMISSIONS' for Air Quality / Emissions, and 'CCEINIT' for Climate Change / Energy Initiatives
* `user_type` - _optional_ - Search by the user type. A single type, or a comma-separate list of multiple types, may be given. Values and what they stand for are as follows: 'IND' for Vehicle Owner/Driver, 'FLEET' for Fleet Purchaser/Manager, 'STATION' for Fueling / TSE Infrastructure Owner, 'AFP' for Alternative Fuel Producer, 'AFS' for Alternative Fuel Dealer, 'PURCH' for Alternative Fuel Purchaser, 'MAN' for AFV Manufacturer/Retrofitter, and 'OTHER' for Other
* `poc` - _optional_ - Include points of contacts in the return value.
* `recent` - _optional_ - Return only recently added or updated laws and incentives
* `expired` - _optional_ - Show only expired, repealed or archived laws and incentives.
* `law_type` - _optional_ - Search by the law type. A single type, or a comma-separate list of multiple types, may be given. Values are as follows: 'STATEINC' for State Incentives, 'UPINC ' for Utility/Private Incentives, 'LAWREG' for Laws and Regulations, 'INC' for Incentives, 'PROG' for Programs, 'LUP' for Last Updated, 'OVIEW' for Overview, and 'HILITE' for Highlights
* `keyword` - _optional_ - Search laws by keyword in title or text.
* `local` - _optional_ - Show only local examples of laws and incentives.

### Return the law categories for a given category type.

*Tags:* `v1`

#### Input Parameters
* `output_format` - _required_ - Response format
    Possible values: json, xml.
* `type` - _optional_ - Search by the category type.
    Possible values: tech, user, regulation, incentive.

### Get the points of contact for a given jurisdiction.

*Tags:* `v1`

#### Input Parameters
* `output_format` - _required_ - Response format
    Possible values: json, xml.
* `jurisdiction` - _required_ - Return the points of contact for the given Jurisdiction. Jurisdiction must be given as a two character state code (eg, 'CO' for Colorado). A single jurisdiction, or a comma-separate list of multiple jurisdiction, may be given.  Use the code 'US' for federal laws and the code 'DC' for Washington D.C.

### Fetch the details of a specific law given the law's ID.

*Tags:* `v1`

#### Input Parameters
* `output_format` - _required_ - Response format
    Possible values: json, xml.
* `id` - _required_ - The id of the law that you are searching
* `poc` - _optional_ - Include points of contacts in the return value.

## License

**flow**ground :- Telekom iPaaS / nrel-gov-transportation-incentives-laws-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
