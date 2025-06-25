# 🧠 Instruction Parallelism & Superscalar CPU Simulation

This project explores how modern **superscalar CPUs** execute instructions in parallel while handling data and control hazards. We analyze a Python function and simulate how instructions are scheduled, issued, executed, and committed using advanced CPU features.

## 🔍 Key Concepts

* **Instruction-Level Parallelism (ILP)**
* **Data Hazards** (RAW, WAR, WAW)
* **Control Hazards** (branch prediction)
* **Superscalar Execution (multi-issue)**
* **Out-of-Order Execution**
* **Register Renaming**
* **Reorder Buffer (ROB) Simulation**

## 🧩 Code Under Analysis

```python
def do_something(a, b):
  x = a + b
  y = a * b
  z = x / y
  if x > y:
    x = x + 3
  y = y + 2
```
*Credit: Codecademy*

## 📊 Visualizations

* Gantt-style pipeline diagrams showing instruction parallelism
* ROB (Reorder Buffer) state tables with issue, execution, and commit cycles

## 📁 Included Files

* `superscalar_gantt.png` – Execution timeline diagram
* `rob_simulation.py` – Python script modeling the ROB
* `superscalar_report.md` – Markdown writeup for technical blogs or Medium
* `instruction_parallelism.qmd` – Quarto blog post with embedded simulation
* `rob_latex_table.tex` – LaTeX-formatted ROB table for academic reports

## 🚀 Highlights

* Models realistic instruction dispatching and commit via ROB
* Demonstrates how CPUs speculatively execute and recover from branch mispredictions
* Explains how hazards are detected and resolved in real-world pipelines

## 📌 Usage

Use this analysis for:

* Learning how out-of-order CPUs schedule and resolve instruction hazards
* Teaching parallel architecture concepts
* Writing performance-aware low-level software

---

> “Instruction-level parallelism is not just about speed — it’s about making every cycle count.”

---

Let me know if you'd like a separate `README.md` file generated or added to your `.zip` archive.
