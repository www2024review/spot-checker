# spot-checker
Check and save the health status log of spot instances concurrently in VM

---
### Spot Checker Flow
1. User sample the workload set and save as file
2. Setting controller server using VM (The number of CPUs are same as the number of workloads)
3. Send workload file to controller server
4. Controller run spot chekcer experiment with workload file
5. Controller run parallel spot checker servers for 24 Hours
6. Controller save the log file of spot checkers
7. You can analyze the spot checker log as ground truth of spot status at that time