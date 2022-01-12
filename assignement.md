# Introduction

You will be asked to present your results and findings to us (using slides,
text or any other way).

After your presentation we will have a discussion about your results so we can
understand your reasoning, chosen methodologies and technology while working on
the assessment.

# Launching a new service in Production

## Background information

The company is working on a brand new product - Wiki Engine for our clients.
The application code reached all the initial milestones, there's only one small
thing left - running it on the production infrastructure.  You are tasked with
creating the initial version and an overall vision of the production
infrastructure for the app.

## Assignment Part 1

We run most of our services in Kubernetes, so your task is to provide a way for
Wiki Engine to run in Kubernetes:

* Create a Docker image for Wiki Engine
* Create a Helm Chart or a Kubernetes Manifests for Wiki Engine (using ksonnet,
  kustomize etc. is also fine)
* Configure the pods to scale on metrics of your choice
* Allow zero-downtime deployments and maintenance

Requirements:
* Wiki Engine should be reachable via Ingress (Ingress controller of your
  choice)
* Data (wiki pages) persistency across container restarts

## Assignment Part 2

You need to present your vision for the Wiki Engine infrastructure to your
colleagues, prepare a short presentation (slides or just text) on any future
improvements you'd like to plan for Wiki Engine, e.g.:

* How do you see the monitoring setup for Wiki Engine? What metrics would you
  collect?
* How do you see scaling Wiki Engine to multiple underlying VMs?


# Running the application

* Install Golang

* Run the Wiki Engine

console $ cd mx-wiki-engine $ go run main.go $ open
http://localhost:8080/view/newpage ```
We expect you to complete it within a week and send it back to us. We'd prefer it if you shared the results of the assessment in a Git repository on github.com, gitlab.org or bitbucket.org




