# spot-checker-aws
Check and save the health status log of spot instances concurrently in EC2

### How to start?
1. Launch your controller EC2 instance (Ubuntu OS, size is depends on number of workloads)

2. Clone this repository, and run setting
```
git clone https://github.com/www2024review/spot-checker.git
cd spot-checker
cd aws
bash settings.sh
```

3. Configure your AWS credentials
```
aws configure
```

4. Modify boto3 profile, S3 bucket names, and spot running time
```
vi workload_sampling.py
vi spot-health-checker.py
```

5. Run sampling code, or use sample workload data (10 workload)
```
python3 workload_sampling.py
```

6. Check parallel spot execution code, then run!
```
vi run_workload_parallel.sh
./run_workload_parallel.sh
```
