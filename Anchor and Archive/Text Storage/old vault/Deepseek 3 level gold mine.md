Yes, structuring your data into **three interconnected categories** (raw material batches → subprocess batches → product assembly/POS) is a logical and scalable way to model traceability and sustainability impacts. This hierarchy aligns with how materials physically flow through the supply chain, while enabling granular tracking and aggregation. Here’s how to design this:

---

### **1. Raw Material Batches**  
**Definition**: The foundational unit of traceability.  
**Examples**:  
- A 10,000kg batch of organic cotton from Farm X.  
- A 5,000-liter batch of recycled polyester resin from Supplier Y.  

**Data to Collect**:  
- Batch ID (unique identifier).  
- Supplier/farm details (location, certifications).  
- Total batch quantity.  
- Environmental impact data (water use, CO₂, land use, etc.).  
- Annual output of the supplier (to calculate your % share if you don’t use the full batch).  

**Key Role**:  
- Serves as the "source of truth" for upstream impacts.  

---

### **2. Material Subprocess Batches**  
**Definition**: Batches created during intermediate processing steps (e.g., spinning, dyeing, finishing).  
**Examples**:  
- A 2,000kg batch of yarn spun from raw cotton.  
- A 500kg batch of dyed fabric (combining yarn + dyes/chemicals).  

**Data to Collect**:  
- Subprocess Batch ID.  
- Input materials (linked to raw material batches or prior subprocess batches).  
- Process details (factory, energy use, waste, chemicals).  
- Output quantity (e.g., 2,000kg of yarn from 2,200kg of cotton, with 200kg waste).  
- Impact data specific to the subprocess (e.g., dyeing emissions).  

**Key Role**:  
- Captures transformations and additive impacts (e.g., energy for dyeing, chemical use).  
- Enables tracking of blended/mixed materials (e.g., fabric blends).  

---

### **3. Product Assembly (PO/Production Order)**  
**Definition**: The final manufacturing step where materials are turned into products.  
**Examples**:  
- A PO for 1,000 T-shirts using 500kg of dyed fabric.  

**Data to Collect**:  
- PO/Style ID.  
- Materials consumed (linked to subprocess batches).  
- Quantity used per product (e.g., 0.5kg fabric per T-shirt).  
- Factory assembly impacts (cut/sew energy, labor, waste).  

**Key Role**:  
- Aggregates all upstream impacts (raw + subprocesses) into the final product.  
- Links sustainability data to commercial transactions (e.g., customer orders).  

---

### **How They Link Together**  
1. **Raw Material Batch → Subprocess Batch**  
   - Example: 10,000kg cotton batch → 8,000kg yarn (after spinning waste).  
   - Impact allocation: The yarn inherits the cotton’s impact + spinning energy.  

2. **Subprocess Batch → Product Assembly (PO)**  
   - Example: 8,000kg yarn → 500kg dyed fabric → 1,000 T-shirts.  
   - Impact allocation: Each T-shirt’s footprint includes cotton growing, spinning, dyeing, and assembly.  

3. **PO → Reporting**  
   - Aggregate impacts across all POs to calculate total annual footprint.  
   - Drill down into specific batches to identify hotspots (e.g., high-impact dyehouses).  

---

### **Why This Works**  
4. **End-to-End Traceability**  
   - Every product can be traced back to its raw materials and subprocesses.  
   - Critical for compliance (e.g., EU Digital Product Passport).  

5. **Accurate Impact Allocation**  
   - Avoids double-counting or gaps by proportionally assigning impacts (e.g., “We used 30% of this dye batch”).  

6. **Flexibility for Complex Supply Chains**  
   - Handles multi-tier processes (e.g., cotton → yarn → fabric → garment).  
   - Supports blended materials (e.g., 60% recycled polyester + 40% virgin cotton).  

7. **Scalability**  
   - Start with raw materials, then add subprocesses and POs as data maturity grows.  

---

### **Implementation Challenges & Solutions**  
| **Challenge** | **Solution** |  
|----------------|--------------|  
| **Data Complexity** | Use a tiered approach: Prioritize high-impact materials (e.g., cotton, polyester) first. |  
| **Supplier Buy-In** | Provide templates/tools for batch reporting. Start with strategic suppliers. |  
| **System Integration** | Ensure Segura and Centric PLM share common IDs (e.g., material codes, batch IDs). |  
| **Partial Batch Usage** | Calculate your % of the batch and apply it to impact metrics (e.g., 5% of a dye batch = 5% of its emissions). |  
| **Missing Data** | Use fallback proxies (e.g., regional averages) flagged as “estimated” in reports. |  

---

### **Tools to Enable This**  
8. **Blockchain/IoT**: Automate batch tracking (e.g., RFID tags for raw cotton bales).  
9. **Digital Twins**: Model subprocesses (e.g., simulate dyeing energy use).  
10. **PLM Integration**: Embed batch/impact data into Centric for designers to prioritize sustainable materials.  

---

### **Example Workflow**  
11. **Raw Material**: Supplier provides Batch #123 (1,000kg organic cotton, 500kg CO₂ footprint).  
12. **Subprocess**: Factory spins Batch #123 into 800kg yarn, adding 100kg CO₂ (spinning energy). Total CO₂ = 600kg.  
13. **Product Assembly**: Your PO uses 400kg of this yarn (50% of the subprocess batch).  
   - Allocated CO₂ = 50% of 600kg = 300kg.  
   - Each T-shirt (0.4kg yarn) = 0.3kg CO₂ from raw + subprocess.  

---

### **Conclusion**  
This three-tiered model is **not just suitable—it’s industry-leading**. By decoupling transactional data (POs) from sustainability data (batches), you future-proof your system for regulations, customer demands, and circularity (e.g., recycling tracking). Start by mapping raw materials and subprocesses, then link them to POs—it’s far more efficient than retrofitting PO-level data later.  

The key is to **build the structure now**, even if you populate it gradually. This avoids the "reinventing the wheel" problem and positions your company as a sustainability leader.