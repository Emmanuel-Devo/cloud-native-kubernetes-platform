# Cloud-Native Kubernetes Platform

A containerized web application deployed on a local Kubernetes cluster using Docker, Kind, Kubernetes Services, NGINX Ingress, health probes, Metrics Server, and Horizontal Pod Autoscaling.

## Project Overview

This project demonstrates a practical Kubernetes deployment workflow from containerization to application routing and autoscaling.

The application is packaged as an NGINX Docker image and deployed to a local Kind Kubernetes cluster.

## Architecture

```text
User
  |
  v
NGINX Ingress Controller
  |
  v
Kubernetes Ingress
  |
  v
web-app-service
  |
  +--------+--------+
  |                 |
  v                 v
Web App Pod      Web App Pod
  NGINX             NGINX
