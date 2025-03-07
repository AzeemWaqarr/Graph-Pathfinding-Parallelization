# 🚀 Graph Pathfinding with Parallelization  

This project implements **Dijkstra's Algorithm** and **Yen’s K Shortest Paths Algorithm** to compute shortest paths in a weighted graph. The solution is designed in both **Serial** and **Parallel** versions, utilizing **OpenMP** and **MPI** for parallel execution.

## 📌 Features  

### ✅ Serial Implementation (`Serial.cpp`)  
- Implements **Dijkstra's Algorithm** for single-source shortest paths  
- Implements **Yen’s Algorithm** to find K-shortest paths  
- Reads graph data from a CSV file (`doctorwho.csv`)  
- Outputs shortest paths along with their total weights  

### ⚡ Parallel Implementation (`Parallel.cpp`)  
- **Parallelized using OpenMP** for multi-threading  
- **Distributed computation using MPI** for multi-node execution  
- Load balancing to divide pathfinding tasks across multiple threads/processes  
- Demonstrates **speedup and efficiency** over the serial version  

---

## 📊 Performance Comparison  

| Execution Type  | Time Taken (ms) |  
|----------------|---------------|  
| Serial Execution  | XXX ms |  
| Parallel Execution (OpenMP + MPI)  | XXX ms |  

The parallelized version achieves significant **speedup** due to distributed workload processing.

---

## 🛠 Technologies Used  

- **Programming Language:** C++  
- **Parallelization Libraries:** OpenMP, MPI  
- **Data Structures:** Unordered Maps, Priority Queues  
- **File Handling:** CSV Parsing for Graph Input  

---

## 📂 Project Structure  
Graph-Pathfinding-Parallelization/ │── Serial.cpp # Serial version using Dijkstra's & Yen's Algorithm
│── Parallel.cpp # Parallelized version using OpenMP & MPI
│── readme.txt # Compilation & Execution instructions
│── doctorwho.csv # Sample dataset for graph input
│── report.pdf # Analysis and insights on performance
│── results/ # Benchmark results & execution logs

---

## 🚀 How to Run  

### **1️⃣ Running the Serial Version**  
#### 💻 Compile:  
g++ -o serial_exec Serial.cpp
#### ▶ Execute:
./serial_exec
You can modify the K value inside Serial.cpp to adjust the number of shortest paths.

#### **2️⃣ Running the Parallel Version**
#### 💻 Compile:
mpic++ -fopenmp Parallel.cpp -o parallel_exec
#### ▶ Execute with MPI:
mpiexec -n 10 ./parallel_exec

## 📜 Report & Analysis
A detailed performance analysis comparing serial and parallel execution is included in report.pdf.
It discusses:

1. Time Complexity of algorithms
2. Speedup gains from parallel execution
3. Scalability of the approach

## 📌 Future Enhancements
✅ Further optimization for load balancing in MPI
✅ Support for larger datasets & real-world graphs
✅ Implement additional shortest path algorithms

## 🤝 Contribution
🔹 Feel free to fork the repo and propose enhancements!
