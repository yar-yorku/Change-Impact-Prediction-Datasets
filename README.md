# Towards a Robust On-line Performance Model Identification Change Impact Prediction Dataset

This repository contains the datasets used to train/test our models in the paper titled "Towards a Robust On-line Performance Model Identification Change Impact Prediction Dataset". 

There are three main directories. The first directory contains the O<sub>0</sub> datasets for when the in-production application, Acme-Air, is only running on our environment. The second directory contains the O<sub>t</sub> datasets where the LAS is deployed alongside Acme-Air. The third directory contains the dataset where the co-located IoT application is deployed alongside Acme-Air, and its measured response time is compared with the predicted response time from our LAS-based model. Inside each directory, the raw dataset from Prometheus/Grafana and dataset with Response Time from HTTPerf for the Light, Medium and Heavy workloads are located. 

### Data Structure

Raw
- Acme Web CPU Usage
- Acme Web Memory Usage
- Acme Web Memory Usage
- MongoDB CPU Usage
- MongoDB Memory Usage
- Avg Host CPU Usage
- Host CPU 0 Usage
- Host CPU 1 Usage
- Host Mem Usage
- Host Mem Total

- VM 1 Avg Host CPU Usage
- VM 1 Host CPU 0 Usage
- VM 1 Host CPU 1 Usage
- VM 1 Host Mem Usage
- VM 1 Host Mem Total
- VM 2 Avg Host CPU Usage
- VM 2 Host CPU 0 Usage
- VM 2 Host CPU 1 Usage
- VM 2 Host Mem Usage
- VM 2 Host Mem Total

Httperf
- NumOfRequests
- Period
- Throughput
- Response Time
