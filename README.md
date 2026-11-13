# 🌾 Agricultural Microcredit Analysis — Senegal (2019–2023)

A Power BI analysis of an NGO microcredit programme for farmers across Senegal's five main agro-ecological zones. The goal: understand how credit relates to productivity, repayment behaviour and economic performance.

## The question

> Does access to microcredit improve farmers' yields, and who repays best?

## Data

Relational dataset (CSV), **50 farmers · 5 years · 15 crops · 370 yearly records**, modelled as a **star schema**:

```
                 DimCulture
                     │
DimRegion ── DimVille ── DimFermier ── FaitAgriculture (fact)
```

| Table | Content |
|---|---|
| `FaitAgriculture` | One row per farmer × crop × year: area (km²), yield, credit amount, amount repaid |
| `DimFermier` | Farmer → region and city |
| `DimCulture` | Crop reference (rice, groundnut, cashew, onion…) |
| `DimRegion`, `DimVille` | Geographic hierarchy (5 zones, 16 cities) |

## Method

1. **Data modelling** in Power Query: typing, relationships, star schema
2. **DAX measures**: total credit, repayment rate, average yield, credit adoption rate, year-over-year change
3. **Dashboard**: KPIs and breakdowns by zone, crop and year, cross-analysis credit × yield

## Key findings

- **≈ 90 M FCFA** disbursed, **≈ 78 %** repaid overall
- Credit was used in **≈ 53 %** of farmer-crop-years
- Repayment varies more by zone than yield does: **Casamance (~83 %)** and **Sénégal Oriental (~82 %)** repay best, **Zone des Niayes (~69 %)** and **Vallée du Fleuve (~72 %)** lowest
- Highest average yields: **groundnut, onion, green beans**
- **No measurable link between credit amount and yield** (correlation ≈ 0). In this data, credit alone does not explain productivity, which points to other factors (crop, practices, inputs) worth investigating

## Repository

| File | Description |
|---|---|
| `agriculture_dashboard.pbix` | Power BI report |
| `*.csv` | Source tables |
| `CHALLENGE DATA – AGRICULTURE.txt` | Challenge brief (in French) |

## How to open

1. Install **Power BI Desktop**
2. Open `agriculture_dashboard.pbix`
3. If prompted, point the data sources to the CSV files in this folder (Power Query → Data source settings)

## Tech

Power BI Desktop · Power Query · DAX · star-schema data modelling

---

**Solange Ilinga** · [LinkedIn](https://linkedin.com/in/solange-ilinga)
