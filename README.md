# Africa Area Data

**Africa Area Data** is an **open-source project** that centralizes, structures, and makes accessible **all administrative geographic divisions of Africa**, from countries, regions, and counties to districts, communes, neighborhoods, and villages. All data uses a **single, standardized JSON format** for consistency and ease of use.

---

## Goal

Administrative geographic data in Africa is often **hard to find**, **incomplete**, or **scattered across multiple sources**. This project aims to:

* **Collect** reliable geographic data for every African country;
* **Standardize** all divisions into a **single JSON structure**, making it easy to use for developers, researchers, and institutions;
* **Share openly** to promote transparency, research, and innovation with open data in Africa.

---

## JSON Structure

Every geographic entity uses the same JSON structure. All fields below are optional except `name`, `type`, `parent`, and `code`:

| Field                       | Description                                                              | Example                                                            |
| --------------------------- | ------------------------------------------------------------------------ | ------------------------------------------------------------------ |
| `name`                      | Official name of the zone                                                | `"Dakar"`                                                          |
| `type`                      | Type of zone (country, region, department, commune, neighborhood…)       | `"region"`                                                         |
| `parent`                    | Code of the parent division (null if top-level)                          | `"SN"`                                                             |
| `code`                      | Unique identifier for the division                                       | `"SN-DAK"`                                                         |
| `alt_names`                 | Alternative or historical names (useful for search or matching)          | `["Dakar Capital Region", "Région de Dakar"]`                      |
| `iso_code`                  | Official ISO code for countries or subdivisions, if available            | `"SN-DAK"`                                                         |
| `population`                | Number of inhabitants (census or estimated)                              | `1050000`                                                          |
| `area_km2`                  | Area in square kilometers                                                | `547`                                                              |
| `coordinates`               | Approximate geographical coordinates (latitude/longitude)                | `{"lat": 14.6928, "lng": -17.4467}`                                |
| `bounding_box`              | Geographic bounding box (useful for mapping/GIS)                         | `{"north": 14.83, "south": 14.66, "east": -17.35, "west": -17.55}` |
| `timezone`                  | Time zone                                                                | `"GMT+0"`                                                          |
| `created_at` / `updated_at` | Creation date / last update of the data                                  | `"2025-01-01" / "2025-10-01"`                                      |
| `links` / `source`          | URL or reference of official source (INS, OCHA, UN, etc.)                | `["https://www.stat-sn.gov.sn/"]`                                  |
| `notes`                     | Additional information or context (e.g., disputed areas, recent changes) | `"Capital region of Senegal"`                                      |
| `neighbors`                 | Codes of neighboring zones (useful for geographic analysis)              | `["SN-THI", "SN-RUF"]`                                             |

---

### Example

```json
{
  "name": "Dakar",
  "alt_names": ["Dakar Capital Region", "Région de Dakar"],
  "type": "region",
  "parent": "SN",
  "code": "SN-DAK",
  "iso_code": "SN-DAK",
  "population": 1050000,
  "area_km2": 547,
  "coordinates": {"lat": 14.6928, "lng": -17.4467},
  "bounding_box": {"north": 14.83, "south": 14.66, "east": -17.35, "west": -17.55},
  "timezone": "GMT+0",
  "status": "recognized",
  "created_at": "2025-01-01",
  "updated_at": "2025-10-01",
  "links": ["https://www.stat-sn.gov.sn/"],
  "notes": "Capital region of Senegal",
  "neighbors": ["SN-THI", "SN-RUF"]
}
```

---

## Possible Uses

* Mapping and GIS (Geographic Information Systems)
* Development of government or civic applications
* Data science and territorial analysis projects
* Visualization and geolocation of public infrastructure
* Demographic, electoral, or economic studies

---

## Contribution

Contributions are **welcome from everyone**! You can:

* Add or correct data for any country;
* Improve JSON structures or consistency;
* Help with documentation and source validation.

---

## Vision

To create **the largest open-source geographic database of the African continent**, reliable, accessible, and interoperable, supporting technological development and territorial knowledge across Africa.
