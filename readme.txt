To run Serial Program:
Compile using: g++ -o S Serial.cpp
Execute using: ./S
You can modify k value inside Serial.cpp to print the number of paths you want


To run Parallel Program:
Compile using: mpic++ -fopenmp Parallel.cpp 
Execute using: mpiexec -n 10 ./a.out
You can modify k value inside Parallel.cpp to print the number of paths you want


