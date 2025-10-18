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
- [ ] Add error handling and logging (`log` + `fern`).
- [ ] Write unit/integration tests for Rust modules.

### **Frontend (Vue.js/TypeScript/D3js)**
- [ ] Set up Vue.js 3 + TypeScript (Pinia/Vuex).
- [ ] Design UI framework (naiveUI).
- [ ] Integrate D3js for dynamic graphics

### **Database (DuckDB)**
- [ ] Integrate DuckDB (in-memory + persistent storage).
- [ ] Implement connection pooling and benchmark performance (hyperfine).
- [ ] Support schema management, indexing, and export/import (Parquet, CSV).

### **Python Integration (Sidecar)**
- [ ] Args management for launching python
- [ ] Executable generation and update
- [ ] Create Python modules for:
  - Data preprocessing (Dask/Polars)
  - ML (Scikit-learn)
- [ ] Implement data serialization (Arrow/JSON) between Rust and Python.

---

## **⚡ Phase 2: Performance & Optimization**
### **Memory Management**
- [ ] Implement RAM monitoring and alerts (e.g., >80% usage).
- [ ] Add options to:
  - Limit dataset size in memory
  - Use DuckDB disk storage for large datasets
  - Clear cache manually/automatically
- [ ] Profile memory with Valgrind (Rust)

### **Computation**
- [ ] Dask vs Polars
- [ ] Implement lazy evaluation and chunked processing.
- [ ] Optimize DuckDB queries (partition pruning, predicate pushdown).

### **Visualization**
- [ ] Establish methods to plot large data
- [ ] Fluidity test

---


## **🧪 Phase 3: Testing & Quality** *(Not now)*
- [ ] Write end-to-end tests (Cypress) for:
  - Data import → query → visualization → export
  - Memory limits and error handling
- [ ] Set up CI/CD (GitHub Actions) for linting, testing, and builds.
- [ ] Add error reporting (Sentry).

---

## **📚 Phase 4: Documentation** *(Not now)*
- [ ] Write user docs:
  - Getting started guide
  - Tutorials (joining datasets, ML models)
  - API reference
- [ ] Create contributor guidelines.
- [ ] Generate inline code docs (`rustdoc`, TypeDoc).

---

## **💬 Phase 5: Community advice** *(Not now)*
- [ ] Set up Discord community.
- [ ] Ask for feedback on reddit, discord...

---


## **📦 Phase NP: Deployment** *(Not a priority)*
- [ ] Package app for Windows (.msi/.exe), macOS (.dmg), Linux (.deb/.rpm).
- [ ] Set up auto-updates (Tauri updater).
- [ ] Launch landing page with downloads, docs, and community links.

---


## **🌥️ Phase Z: Future-Proofing** *(Much later)*
- [ ] Design plugin architecture for cloud backends (Spark, Airflow, minIO).
- [ ] Plan for distributed computing (Dask cluster, Ray).
---
