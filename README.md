# Exam-Scheduling-using-Genetic-Algorithm-GA-
This project implements an Exam Scheduling System using a Genetic Algorithm (GA) to generate an optimal timetable while satisfying hard constraints and optimizing soft constraints.


# 📘 Exam Scheduling using Genetic Algorithm (GA)

This project implements an **Exam Scheduling System** using a **Genetic Algorithm (GA)** to generate an optimal timetable while satisfying **hard constraints** and optimizing **soft constraints**.
The solution evolves multiple populations of exam schedules and selects the best timetable based on a fitness function.

---

## 🧠 Problem Overview

The goal is to automatically generate an exam timetable such that:

### ✅ Hard Constraints (Must be satisfied)

* Every course has exactly one exam.
* No student has overlapping exams.
* Exams are scheduled only on weekdays (Monday–Friday).
* Exam timings are between **9:00 AM – 5:00 PM**.
* Each exam has an invigilating teacher.
* No teacher has consecutive invigilation duties.

### 🎯 Soft Constraints (Optimization Goals)

* Common break on **Friday (1–2 PM)**.
* Avoid back-to-back exams for students.
* Management (MG) exams before Computer Science (CS) exams.
* Faculty meeting slots where at least half of the faculty is free.

---

## 🛠️ Technologies & Libraries Used

### Programming Language

* **Python 3.8+**

### Required Python Libraries

Install the following libraries before running the notebook:

```bash
pip install numpy pandas tabulate
```

#### Library Usage

| Library    | Purpose                                        |
| ---------- | ---------------------------------------------- |
| `numpy`    | Random selection, probability handling         |
| `pandas`   | Dataset handling (students, courses, teachers) |
| `random`   | Genetic Algorithm operations                   |
| `tabulate` | Displaying schedules in table format           |
| `jupyter`  | Running the notebook                           |

---

## ⚙️ Environment Setup

### 1️⃣ Install Python

Make sure Python **3.8 or above** is installed:

```bash
python --version
```

### 2️⃣ (Optional) Create Virtual Environment

```bash
python -m venv ga_env
source ga_env/bin/activate   # Linux/Mac
ga_env\Scripts\activate      # Windows
```

### 3️⃣ Install Dependencies

```bash
pip install numpy pandas tabulate jupyter
```

---

## 📂 Project Structure

```
Exam-Scheduling-GA/
│
├── Asg03-22I-1711.ipynb   # Main implementation notebook
├── log.txt               # Fitness logs for each generation
├── courses.csv           # Course data
├── studentCourse.csv     # Student-course mapping
├── studentNames.csv      # Student list
├── teachers.csv          # Teacher list
└── README.md             # Project documentation

```

---

## ▶️ How to Run the Project

### 1️⃣ Launch Jupyter Notebook

```bash
jupyter notebook
```

### 2️⃣ Open the Notebook

Open:

```
main.ipynb
```

### 3️⃣ Run All Cells

* Click **Kernel → Restart & Run All**
* Or press **Shift + Enter** cell-by-cell

---

## 🎮 How the System Works (Execution Flow)

1. Load datasets (courses, students, teachers)
2. Generate **initial random populations**
3. Evaluate fitness for each population
4. Apply:

   * **Roulette Wheel Selection**
   * **Crossover**
   * **Mutation**
5. Evolve over **multiple generations**
6. Display:

   * Fitness scores per generation
   * Best timetable
   * Hard & soft constraint compliance
7. Save fitness logs to `log.txt`

---

## 📊 Output

* Tabulated exam schedules
* Generation-wise fitness comparison
* Best timetable with highest fitness score
* Constraint satisfaction summary
* Detailed logs saved in `log.txt`

---

## 🧪 Customization Options

You can easily modify:

* Number of generations
* Population size
* Mutation rate
* Time slots, rooms, or constraints
* Fitness reward/penalty weights

---

## 📌 Notes

* This solution is **heuristic-based**, not brute-force.
* Genetic Algorithms provide **near-optimal** solutions efficiently.
* Best suited for **large scheduling problems**.

---

## 📌 Author

Bachelor’s in Cyber Security


## 📄 License

This project is for **educational purposes only**.
