# GPU Kubernetes Lab on GCP

This project simulates a GPU-accelerated Kubernetes environment using **Terraform** and **GCP**, designed as a proof-of-concept for high-performance AI/ML container workloads using **NVIDIA GPU Operator**, **DCGM**, and custom GPU workloads.

---

## 🎯 Objectives

- Provision GPU-enabled nodes in Google Cloud
- Set up a Kubernetes cluster ready for GPU workloads
- Deploy the **NVIDIA GPU Operator** to expose GPU resources
- Run a sample containerized GPU job (`nvidia-smi`)
- Monitor GPU metrics using **DCGM Exporter**
- Support MIG, policy enforcement, and multi-tenant prep

---

## 🚀 Quick Start

### 1. Configure GCP & Terraform
```bash
cd terraform
terraform init
terraform apply -var="project_id=your-gcp-project-id"
