# ArgoCD App-of-Apps Pattern

This repository demonstrates the **ArgoCD App-of-Apps pattern**, a scalable GitOps approach for managing and deploying multiple Kubernetes applications using a single parent ArgoCD application.

The pattern is widely adopted in **enterprise Kubernetes platforms** to achieve centralized control, consistency, and operational efficiency.

---

## 🚀 Overview

The App-of-Apps pattern uses:
- A **root (parent) ArgoCD Application**
- Multiple **child ArgoCD Applications** referenced from the parent

This enables modular, repeatable, and scalable application lifecycle management across environments such as **dev, staging, and production**.

---

## 🧩 How It Works

1. A **parent application** is created in ArgoCD.
2. The parent references a Git directory or repository containing multiple child application manifests.
3. Each **child application** manages a single workload or component.
4. ArgoCD continuously reconciles the desired state from Git.

---

## ✨ Highlights

- Centralized deployment using a single parent ArgoCD application
- Each application managed as an independent child app
- Declarative GitOps model – Git as the single source of truth
- Automatic sync, health monitoring, and self-healing
- Simplified onboarding of new applications
- Clear separation of platform components and business workloads
- Improved visibility with application-level and pod-level health status

---

## ✅ Key Benefits

- Scales effortlessly as the number of applications grows
- Reduces operational overhead for large Kubernetes clusters
- Enables standardized deployments across dev, staging, and prod
- Ideal for platform engineering and enterprise GitOps adoption
- Faster recovery and drift detection through ArgoCD reconciliation

---

## 🛠 Tech Stack

- Kubernetes
- Argo CD
- GitOps

---

## 📌 Use Cases

- Platform engineering teams
- Multi-team Kubernetes environments
- Large-scale microservices deployments
- Standardized GitOps workflows

---
⭐ If you find this repository useful, consider starring it!
