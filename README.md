# Monitoring with Prometheus + Grafana

Built a full observability stack using Prometheus and Grafana to monitor a Python Flask application running on Kubernetes.

## What I Built
- Flask app exposing custom metrics at /metrics endpoint
- Prometheus scraping app metrics every 15 seconds
- Grafana dashboard connected to Prometheus as data source
- Kubernetes deployments for app, Prometheus, and Grafana
- Pod annotations for automatic Prometheus service discovery

## Metrics Tracked
- Total request count per endpoint
- Request latency in seconds
- Application health status

## GitOps Flow
App exposes /metrics → Prometheus scrapes → Grafana visualizes

## Tech Stack
Prometheus · Grafana · Kubernetes · Docker · Python Flask · prometheus-client

## Folder Structure
- app/ — Flask app with Prometheus metrics instrumentation
- k8s/ — Kubernetes manifests for app deployment
- k8s/monitoring/ — Prometheus config and Grafana deployment
