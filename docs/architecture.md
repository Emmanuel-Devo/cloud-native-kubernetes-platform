# Architecture

## Overview

This project demonstrates a containerized web application deployed on a local Kubernetes cluster using Docker and Kind.

## Architecture Flow

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
  v
+---------------------------+
|                           |
v                           v
Web App Pod              Web App Pod
NGINX                    NGINX
