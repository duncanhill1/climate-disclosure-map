# Disclosure Data Format

Each jurisdiction record should use the following structure:

- id: unique identifier
- type: "country" or "state"
- name: jurisdiction name
- parentCountry: optional, used for states or regions
- isoCode: ISO country or subnational code where possible
- disclosureTitle: short name of the law, rule, or framework
- summary: 1 to 3 sentence explanation
- officialUrl: government or official regulatory source
- status: "active", "proposed", or "partial"
- coordinates: optional longitude/latitude array for markers

## Example

```json
{
  "id": "us-ca",
  "type": "state",
  "name": "California",
  "parentCountry": "United States",
  "isoCode": "US-CA",
  "disclosureTitle": "SB 253 and SB 261",
  "summary": "California climate disclosure laws affecting certain large companies doing business in the state.",
  "officialUrl": "https://leginfo.legislature.ca.gov/",
  "status": "active",
  "coordinates": [-119.4179, 36.7783]
}
