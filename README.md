# Data Contracts

A data contract is a document that defines **the ownership, structure, semantics, quality, and terms of use** for exchanging data between a data producer and their consumers.
This repository contains **Data Contracts** defined using the **Open Data Contract Standard (ODCS)**.  

---

## 📌 Purpose

- Standardize how datasets are defined and governed
- Ensure consistent data structure and interpretation across teams
- Enable executable data quality validation
- Support data governance, monitoring, and accountability

---

## 📄 ODCS as the Data Contract Standard

Open Data Contract Standard (ODCS) is used as the official standard to define data contracts. 

Why ODCS?
- *Industry Standard*
  
  Open, vendor-neutral, and led by the Linux Foundation (Bitol)
- *Business & Technical Aligned*
  
  Clearly defines ownership, schema, quality rules, and usage
- *Tool-Friendly*
  
  Works well with DataHub, GX, and Github
- *Scalable & Governed*
  
  Supports versioning, lifecycle status, and change control

---

## 🛡️ Data Contract Implementation Scope
Critical datasets & critical data elements (CDE)
Why the Scope Is Limited to Critical Datasets & CDEs :
- *Business Impact Is Highest*

  Focus on areas with highest risk and value to the business
- *Faster & More Realistic Implementation*

  Allows a practical and incremental approach with faster results
- *Align with Data Governance Best Practices*

  Not all data needs to be controlled at the same level.

---

## 🔁 Data Contract Life-cycle
Data contracts are **living artifacts**, not static documents. 

Each data contract follows a controlled lifecycle to ensure governance, accountability, and auditability.
### **1. Proposed**
- A new data contract is proposed by the data producer
- Initial definitions of schema, ownership, and rules
- Not yet reviewed or enforced

### **2. Draft**
- The contract is being refined
- Under technical and business discussion
- Not yet used for validation or monitoring

### **3. Active**
- The contract is officially approved and enforced
- Data quality rules are executed
- Validation results are monitored

### **4. Deprecated**
- The contract is still available but no longer recommended
- Usually replaced by a newer version
- Maintained temporarily for backward compatibility

### **5. Retired**
- The contract is no longer used
- Dataset is discontinued or replaced
- Contract is kept for historical reference and audit purposes

**Lifecycle Flow:**  
`Proposed → Draft → Active → Deprecated → Retired`

This lifecycle supports:
- Controlled change management  
- Clear ownership and accountability  
- Compliance with data governance best practices

---
## 📂 Repository Structure

```text
data-contracts/
├── templates/
│   └── odcs-template.yaml
|   └── odcs-example.yaml
├── data-contracts/
│   └── <database-name>/
│       └── <table_name>.yaml
└── README.md
