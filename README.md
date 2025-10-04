Automate CATIA with Python | PyCATIA Tutorial 🚀

This repository contains all the files and code examples from my YouTube tutorial on automating CATIA design using Python and the PyCATIA library.

## 📌 What’s inside?
- Jupyter Notebook (.ipynb) with step-by-step code


## 🔧 Requirements
- CATIA V5 installed
- Python 3.x
- PyCATIA library


✅ Why This Matters?

Automating CATIA workflows with Python saves time, reduces repetitive work, and generates valuable data for analysis and machine learning applications — the same approach top OEMs use.


---

# 🚀 PyCATIA Cheatsheet – Roadmap for Automation

This cheatsheet gives you a **quick overview of the most useful PyCATIA modules** and when to use them.  
Perfect for practicing automation scripts in **CATIA V5**.

---

## 1️⃣ Getting Started
- **`pycatia`**
  - Entry point → `from pycatia import catia`
  - Access **Application**, **Documents**, **Windows**, **Settings**

---

## 2️⃣ Mechanical Design
- **`mec_mod_interfaces`**
  - Create Pads, Pockets, Shafts, etc. in **Part Design**
- **`sketcher_interfaces`**
  - Work with **Sketches** (lines, circles, constraints)
- **`part_interfaces`**
  - Manage Bodies, Features, and Parameters inside a Part

---

## 3️⃣ Assembly Design
- **`product_structure_interfaces`**
  - Work with Product Trees  
  - Insert Parts, move items, edit properties
- **`assembly_interfaces`**
  - Create and manage **Assembly Constraints**

---

## 4️⃣ Drafting
- **`drafting_interfaces`**
  - Create and edit **Drawings**
- **`drafting_2dL_interfaces`**
  - Low-level control of **2D Geometry**

---

## 5️⃣ Selection & Visualization
- **`in_interfaces.selection`**
  - Select Features, Bodies, Sketches, or Products
- **`in_interfaces.vis_property_set`**
  - Change **Color, Line Thickness, Transparency**

---

## 6️⃣ Knowledgeware (Parameters & Rules)
- **`knowledge_interfaces`**
  - Create Parameters and Formulas
- **`general_knowledge_interfaces`**
  - Work with **Rules, Checks, Relations**

---

## 7️⃣ Analysis & Measurements
- **`analysis_interfaces`**
  - Run mechanical analyses
- **`space_analyses_interfaces`**
  - Measure **Distance, Angle, Mass, Inertia**
- **`enumeration`**
  - Useful **Enums** (geometry types, constraint types, etc.)

---

## 8️⃣ Advanced Use Cases
- **`kinematics_interfaces`**
  - Simulate **Mechanisms**
- **`simulation_interfaces`**
  - Run simulations
- **`dnb_robot_interfaces`**
  - Robot Simulation
- **`composites_interfaces`**
  - Composite Design
- **`manufacturing_interfaces`** / **`surface_machining_interfaces`**
  - NC Programming & Machining Automation

---

## 📌 How to Decide Which Module to Use?
- Change **Part color** → `in_interfaces.selection` + `vis_property_set`  
- Create a **Pad** → `mec_mod_interfaces`  
- Measure **distance** → `space_analyses_interfaces`  
- Create **parameter/formula** → `knowledge_interfaces`  

---

💡 Tip: This roadmap is great for **learning, testing, and building reusable scripts**.  
Use it as a quick reference when you’re not sure which module to import.

---

✍️ Maintainer: *Sheyda Karimabadi*  
🔗 Related repo: [PyCATIA GitHub](https://github.com/evereux/pycatia)  

---

## 📝 Notes & Caveats  

- **Modules**: Module and interface names (e.g., `mec_mod_interfaces`, `part_interfaces`, `sketcher_interfaces`, `in_interfaces.selection`) are taken directly from PyCATIA.  
- **Categorization**: The grouping into sections (Mechanical, Assembly, Drafting, Visualization, etc.) is **not part of the official docs**. It’s added here for **better learning and quicker reference**.  
- **Examples**: Code snippets (e.g., change color, selection, Pad creation, Measure Distance) are valid and executable with the corresponding modules.  
- ⚠️ **Module Overlap**: Some modules overlap in functionality. For example, both `general_knowledge_interfaces` and `knowledge_interfaces` can be used for parameters and formulas.  
- ⚠️ **CATIA Version**: Not all modules and methods are tested on every version of CATIA. Depending on your CATIA release and COM API settings, certain functions may behave differently or may not be available at all.  

---

Happy learning!
If you find this useful, ⭐ the repo and share your feedback!
