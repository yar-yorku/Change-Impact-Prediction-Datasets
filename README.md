# Towards a Robust On-line Performance Model Identification Change Impact Prediction Dataset

This repository contains the datasets used to train/test our models in the paper titled "Towards a Robust On-line Performance Model Identification Change Impact Prediction Dataset". 

There are three main directories. The first directory contains the O<sub>0</sub> datasets for when the in-production application, Acme-Air, is only running on our environment. The second directory contains the O<sub>t</sub> datasets where the LAS is deployed alongside Acme-Air. The third directory contains the dataset where the co-located IoT application is deployed alongside Acme-Air, and its measured response time is compared with the predicted response time from our LAS-based model. Inside each directory, the raw dataset from Prometheus/Grafana and dataset with Response Time from HTTPerf for the Light, Medium and Heavy workloads are located. 

### Data Structure

General
- Acme Web CPU Usage: CPU utilization percentage of the Acme-Air NodeJS Web Server.
- Acme Web Memory Usage: Memory usage of the Acme-Air NodeJS Web Server.
- MongoDB CPU Usage: CPU utilization percentage of the Acme-Air MondoDB database.
- MongoDB Memory Usage: Memory usage of the Acme-Air MondoDB database.


Raw for 1VM Deployment
- Avg Host CPU Usage: The Virtual Machine Average CPU Utilization.
- Host CPU 0 Usage: The Virtual Machine vCPU Utilization.
- Host CPU 1 Usage: The Virtual Machine vCPU Utilization.
- Host Mem Usage:The Virtual Machine Memory Usage.
- Host Mem Total: The Virtual Machine Total Memory.

Raw for 2VM Deployment
- VM 1 Avg Host CPU Usage: The Virtual Machine Average CPU Utilization for VM1.
- VM 1 Host CPU 0 Usage: The Virtual Machine vCPU Utilization for VM1.
- VM 1 Host CPU 1 Usage: The Virtual Machine vCPU Utilization for VM1.
- VM 1 Host Mem Usage: The Virtual Machine Memory Usage for VM1.
- VM 1 Host Mem Total: The Virtual Machine Total Memory for VM1.
- VM 2 Avg Host CPU Usage: The Virtual Machine Average CPU Utilization for VM2.
- VM 2 Host CPU 0 Usage: The Virtual Machine vCPU Utilization for VM2.
- VM 2 Host CPU 1 Usage: The Virtual Machine vCPU Utilization for VM2.
- VM 2 Host Mem Usage: The Virtual Machine Memory Usage for VM2.
- VM 2 Host Mem Total: The Virtual Machine Total Memory for VM1.

Httperf
- NumOfRequests: Total # of Requests from HTTPerf.
- Period: Specifies the time interval between the creation of connections or sessions (See HTTPerf: https://linux.die.net/man/1/httperf).
- Throughput: # of requests processed per second.
- Response Time: Amount of time (ms) it takes for Acme-Air to respond to a client's request.
