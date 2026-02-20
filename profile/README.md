# 🚀 Red Wing Labs (RWL) Roadmap

## **📌 Phase 1: Core Architecture & Setup** *(Ongoing)*
### **Backend (Rust/Tauri v2)**
- [x] Set up Tauri v2 + Rust project with Vue.js/TypeScript frontend compatibility.
- [ ] Design modular Rust backend for data processing, DuckDB integration, and file I/O.
- [ ] Implement Tauri commands:
  - Data ingestion (CSV, Parquet, JSON)
  - DuckDB query execution
  - Python sidecar communication
  - Resource monitoring (RAM/CPU)

### **Frontend (Vue.js/TypeScript/D3js)**
- [x] Set up Tauri v2 (Rust + Vue.js 3 + TypeScript)
- [ ] Integrate UI framework (naiveUI).
- [ ] Integrate D3js

### **Python Integration (Sidecar)**
- [ ] Args management for launching python
- [ ] Executable generation and update
- [ ] Create Python modules for:
  - Data preprocessing (Dask/Polars)
  - ML (Scikit-learn)
- [ ] Implement data serialization (Arrow/JSON) between Rust and Python.

---

## **⚡ Phase 2: Performance & Optimization**
- [ ] Implement RAM monitoring and alerts.
- [ ] Profile memory with Valgrind (Rust)
- [ ] Dask vs Polars vs Pyspark
---


## **🧪 Phase 3: Testing & Quality** *(Not now)*
- [ ] Write tests (Cypress) for:
  - Data import → query → visualization → export
  - Memory limits and error handling
- [ ] Set up CI/CD (GitHub Actions) for linting, testing, and builds.

---

## **📚 Phase 4: Documentation** *(Not now)*
- [ ] Write user docs (Getting started guide, Tutorials etc)
- [ ] Create contributor guidelines.

---

## **📦 Phase 5: Deployment** *(Not a priority)*
- [ ] Package app for Windows (.msi/.exe), macOS (.dmg), Linux (.deb/.rpm).
- [ ] Set up auto-updates (Tauri updater).
- [ ] Launch landing page with downloads, docs, and community links.

---


## **🌥️ Phase 6: Future-Proofing** *(Much later)*
- [ ] Design plugin architecture for cloud backends (Spark, Airflow, minIO).
---
