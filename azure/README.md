# spot-checker-azure
Check and save the health status log of spot instances concurrently in Azure VM

### How to start?
1. Launch your controller azure VM (Ubuntu OS, size is depends on number of workloads)

2. Clone this repository, and run setting
```
git clone https://github.com/www2024review/spot-checker.git
cd spot-checker
cd azure
bash settings.sh
```

3. Set workloads
```
vi workload.txt
```

4. Check parallel spot execution code, then run!
```
vi run_workload_parallel.sh
./run_workload_parallel.sh
```
