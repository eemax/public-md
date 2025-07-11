- [[1.1 Data]]
## Hierarchy of data
1. Collection/seasons
2. Product data
3. Material/components
4. Sub-processing
5. Raw materials

## Action plan example
1. **Define a Unified Reporting Framework**
	- Establish **standardized templates** for reporting at each hierarchy level. For example:
		- **Collection/Season**: Include collection name, launch year, target regions.
		- **Product Data**: SKU, category, compliance certifications, dimensions, weight.
		- **Material/Component**: Material name, percentage composition, supplier.
		- **Processes**: Type, location, emissions, energy use.
		- **Raw Materials**: Source, certifications (e.g., GOTS, FSC), recyclability.

2. **Adopt Common Data Formats**
	- Use universally accepted file formats (e.g., CSV, JSON, XML) for data exchange between teams and systems.
		- If I enforce excel format with a specific output, then I can later run it through a .py script
	- Ensure that units of measurement (e.g., weight in grams, dimensions in cm) are standardized globally.
3. **Centralize Reporting Standards**
	- Create a **master data dictionary** that defines all terms and fields (e.g., what qualifies as a “process” or “material”).
	- Example:
		- **Material**: “Recycled Polyester” (min 30% post-consumer waste, certified by GRS).
		- **Process**: “Dyeing” (include water usage in liters per kilogram of fabric).

4. **Create Reporting Benchmarks**
	- Define **KPIs** and minimum data quality thresholds for each level.
	- Example KPIs:
		- Material-level: 100% traceability of raw material origins.
		- Process-level: Carbon footprint reported for 80% of manufacturing processes.