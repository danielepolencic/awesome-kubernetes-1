# Kubernetes Monitoring and Logging
- [Introduction](#introduction)
- [Kubernetes Logging](#kubernetes-logging)
- [SLOs in Kubernetes](#slos-in-kubernetes)
- [ECK Elastic Cloud on Kubernetes](#eck-elastic-cloud-on-kubernetes)
- [Telegraf Operator](#telegraf-operator)
- [Monitoring Certificates Expiration](#monitoring-certificates-expiration)
- [Videos](#videos)

## Introduction
* [kube-prometheus](https://github.com/prometheus-operator/kube-prometheus) Use Prometheus to monitor Kubernetes and applications running on Kubernetes. This repository collects Kubernetes manifests, Grafana dashboards, and Prometheus rules combined with documentation and scripts to provide easy to operate end-to-end Kubernetes cluster monitoring with Prometheus using the Prometheus Operator.
    * [prometheus-community/kube-prometheus-stack 🌟🌟](https://artifacthub.io/packages/helm/prometheus-community/kube-prometheus-stack) **kube-prometheus-stack collects Kubernetes manifests, Grafana dashboards, and Prometheus rules combined with documentation and scripts to provide easy to operate end-to-end Kubernetes cluster monitoring with Prometheus using the Prometheus Operator.**
* [medium: Kubernetes Monitoring: Kube-State-Metrics](https://medium.com/@chrisedrego/kubernetes-monitoring-kube-state-metrics-df6546aea324)
* [Kubernetes Monitoring 101 — Core pipeline & Services Pipeline](https://levelup.gitconnected.com/kubernetes-monitoring-101-core-pipeline-services-pipeline-a34cd4cc9627)
* [medium: Utilizing and monitoring kubernetes cluster resources more effectively](https://medium.com/@martin.schneppenheim/utilizing-and-monitoring-kubernetes-cluster-resources-more-effectively-using-this-tool-df4c68ec2053)
* [sysdig.com: Seven Kubernetes monitoring best practices every monitoring solution should enable](https://sysdig.com/blog/kubernetes-monitoring-best-practices/)
* [magalix.com: Best Practices And Tools For Monitoring Your Kubernetes Cluster](https://www.magalix.com/blog/best-practices-and-tools-for-monitoring-your-kubernetes-cluster)
* [sysdig.com: Monitoring Kubernetes in Production](https://sysdig.com/blog/monitoring-kubernetes/)
* [sysdig.com: How to monitor Kubernetes control plane](https://sysdig.com/blog/monitor-kubernetes-control-plane/)
* [thenewstack.io: 12 Critical Kubernetes Health Conditions You Need to Monitor](https://thenewstack.io/12-critical-kubernetes-health-conditions-you-need-to-monitor/)
* [devopscurry.com: Best  Open-Source Monitoring Tools for Kubernetes in 2021](https://devopscurry.com/best-open-source-monitoring-tools-for-kubernetes-in-2021/)
* [circonus.com: 12 Critical Kubernetes Health Conditions You Need to Monitor and Why](https://www.circonus.com/2020/12/12-critical-kubernetes-health-conditions-you-need-to-monitor-and-why/)
* [circonus.com: Guide to Kubernetes Monitoring: Part 1](https://www.circonus.com/2020/09/guide-to-kubernetes-monitoring-part-1/)
    * [circonus.com: Guide to Monitoring Kubernetes, Part 2: Which Metrics and Health Conditions You Should be Monitoring](https://www.circonus.com/2021/01/guide-to-monitoring-kubernetes-part-2-which-metrics-and-health-conditions-you-should-be-monitoring/)
* [infracloud.io: Monitoring Kubernetes cert-manager Certificates with BotKube](https://www.infracloud.io/blogs/monitoring-kubernetes-cert-manager-certificates/) - [botkube.io](https://www.botkube.io/)
* [kube-state-metrics 🌟](https://github.com/kubernetes/kube-state-metrics) **Add-on agent to generate and expose cluster-level metrics. kube-state-metrics is a simple service that listens to the Kubernetes API server and generates metrics about the state of the objects. (See examples in the Metrics section below.) It is not focused on the health of the individual Kubernetes components, but rather on the health of the various objects inside, such as deployments, nodes and pods.**
* [itnext.io: Monitoring Kubernetes Jobs](https://itnext.io/monitoring-kubernetes-jobs-8adc241a7b60)
* [cncf.io: Avoiding Kubernetes cluster outages with synthetic monitoring](https://www.cncf.io/blog/2021/08/10/avoiding-kubernetes-cluster-outages-with-synthetic-monitoring/)
* [medium: Replication Controller & Replica sets in Kubernetes](https://medium.com/avmconsulting-blog/replication-controller-replica-sets-in-kubernetes-820f3cec7170)
* [kubermatic.com: The Complete Guide to Kubernetes Metrics](https://www.kubermatic.com/blog/the-complete-guide-to-kubernetes-metrics/)
* [arabitnetwork.com: K8S – Enabling Auditing Logs | Step-by-Step](https://arabitnetwork.com/2021/03/13/k8s-enabling-auditing-logs-step-by-step/)
* [youtube.com: Cloud Quick POCs - Kubernetes monitoring metrics using Grafana Cloud on AWS EKS | Observability | Grafana](https://www.youtube.com/watch?v=FVDHWPxK5nU&ab_channel=CloudQuickPOCs)
* [loft.sh: Kubernetes Cost Monitoring with Prometheus & Grafana](https://loft.sh/blog/kubernetes-cost-monitoring-with-prometheus-and-grafana/)
* [==anaisurl.com: Full Tutorial: Monitoring and Troubleshooting stack with Prometheus, Grafana, Loki and Komodor== 🌟](https://anaisurl.com/full-tutorial-monitoring/) 
* [==blog.flant.com: Collecting system information from a bunch of Kubernetes clusters==](https://blog.flant.com/collect-system-information-stats-from-kubernetes-clusters/)
* [medium.com/is-it-observable: How to collect metrics in a Kubernetes cluster](https://medium.com/is-it-observable/how-to-collect-metrics-in-a-kubernetes-cluster-9ad4a69aafb0)
* [itnext.io: How to tackle Kubernetes observability challenges with Pixie](https://itnext.io/how-to-tackle-kubernetes-observability-challenges-with-pixie-4c6414ca913)
* [medium.com/@lucapompei91: Kubernetes observability](https://medium.com/@lucapompei91/kubernetes-observability-17a7875a38f6) 
* [==dev.to: Monitoring Kubernetes cluster logs and metrics using Grafana, Prometheus and Loki==](https://dev.to/leroykayanda/kubernetes-monitoring-using-grafana-3dhc)

## Kubernetes Logging 
- [cncf.io: Logging in Kubernetes: EFK vs PLG Stack](https://www.cncf.io/blog/2020/07/27/logging-in-kubernetes-efk-vs-plg-stack/)
- [medium: How to Deploy an EFK stack to Kubernetes](https://medium.com/avmconsulting-blog/how-to-deploy-an-efk-stack-to-kubernetes-ebc1b539d063)
- [digitalocean.com: How To Set Up an Elasticsearch, Fluentd and Kibana (EFK) Logging Stack on Kubernetes](https://www.digitalocean.com/community/tutorials/how-to-set-up-an-elasticsearch-fluentd-and-kibana-efk-logging-stack-on-kubernetes)
- [portworx.com: How to backup and restore Elasticsearch on Kubernetes](https://portworx.com/how-to-backup-and-restore-elasticsearch-on-kubernetes/)
- [elastic.co: Elastic Stack Monitoring with Elastic Cloud on Kubernetes (ECK - official operator)](https://www.elastic.co/es/blog/elastic-stack-monitoring-with-elastic-cloud-on-kubernetes) In this blog post, we'll explore how the official **ElasticCloud** on **Kubernetes operator** can be used to easily deploy and manage **ElasticStack Monitoring** using the new **Beat CRD**.
* [papertrail.com: Quick and Easy Way to Implement Kubernetes Logging](https://www.papertrail.com/blog/quick-and-easy-way-to-implement-kubernetes-logging/) The SolarWinds® Papertrail™ team is excited to announce SolarWinds rKubeLog, an open-source project designed to streamline Kubernetes logging. rKubeLog allows you to forward logs to Papertrail from within a Kubernetes cluster without using a daemon or setting up application-level logging or a logging sidecar.
* [qlinh.com: Leveraging Kubernetes audit logs for threat detection](https://qlinh.com/infosec/2020/09/30/threat-detection-with-kubernetes-audit-logs.html) Kubernetes audit logs can provide great visibility into the operation and inner workings of your cluster. Learn how to leverage Kubernetes audit logs for threat detection
* [itnext.io: Kubernetes Logging in Production](https://itnext.io/kubernetes-logging-in-production-545ea88d9a4a)
* [opensource.com: What you need to know about cluster logging in Kubernetes 🌟](https://opensource.com/article/21/11/cluster-logging-kubernetes) Explore how different container logging patterns in Kubernetes work.
* [==devopscube.com: Kubernetes Logging Tutorial For Beginners== 🌟](https://devopscube.com/kubernetes-logging-tutorial)
* [aws.plainenglish.io: Kubernetes Deep Dive: Log Management](https://aws.plainenglish.io/kubernetes-deep-dive-log-management-a60b06e2d738) Part 28 of a series of articles about learning k8s!
* [medium.com/vmacwrites: Kubernetes Audit Logs: Who created or deleted a namespace?](https://medium.com/vmacwrites/kubernetes-audit-logs-who-created-or-deleted-a-namespace-7d55c20d2730) Learn how to set up log forwarding and collect audit logs that are passed through the Kubernetes API server to IBM Log Analysis to check who initiated a request and when they did so.
* [shivanshu1333.medium.com: Structured logging in Kubernetes](https://shivanshu1333.medium.com/structured-logging-in-kubernetes-58cf35e6d60d)
    * Logs are an essential aspect of observability and a critical tool for debugging. But Kubernetes logs have traditionally been unstructured strings, making any automated parsing difficult and any downstream processing, analysis, or querying challenging to do reliably.
    * In Kubernetes 1.19, we are adding support for structured logs, which natively support (key, value) pairs and object references. We have also updated many logging calls such that over 99% of logging volume in a typical deployment are now migrated to the structured format.
    * To maintain backwards compatibility, structured logs will still be outputted as a string where the string contains representations of those “key”=”value” pairs. Starting in alpha in 1.19, logs can also be outputted in JSON format using the --logging-format=json flag.
* [tealfeed.com: Kubernetes Audit Logs: Who created or deleted a namespace?](https://tealfeed.com/kubernetes-audit-logs-created-deleted-namespace-ho5o3) Learn how to set up log forwarding and collect audit logs that are passed through the Kubernetes API server to IBM Log Analysis to check who initiated a request and when they did so.

## SLOs in Kubernetes
- [==thenewstack.io: Service Level Objectives in Kubernetes==](https://thenewstack.io/service-level-objectives-in-kubernetes/) an SLO is simply a metric, a goal for that metric, and a time period. For instance: “the success rate for service A must be at least 99.7% percent over the past 30 days.” The metric is known as the “service level indicator” (SLI) and the goal is the “objective.”
- [thenewstack.io: SLOs in Kubernetes, 1 Year Later](https://thenewstack.io/slos-in-kubernetes-1-year-later/)

## ECK Elastic Cloud on Kubernetes 
- [elastic.co: How to configure Elastic Cloud on Kubernetes with SAML and hot-warm-cold architecture](https://www.elastic.co/es/blog/how-to-configure-elastic-cloud-on-kubernetes-with-saml-and-hot-warm-cold-architecture) Elastic Cloud on Kubernetes (ECK) is an easy way to get the Elastic Stack up and running on top of Kubernetes. That’s because ECK automates the deployment, provisioning, management, and setup of Elasticsearch, Kibana, Beats, and more. 

## Telegraf Operator
- [influxdata.com: Expand Kubernetes Monitoring with Telegraf Operator](https://www.influxdata.com/blog/expand-kubernetes-monitoring-telegraf-operator)

## Monitoring Certificates Expiration
- [itnext.io: Monitoring Certificates Expiration in Kubernetes with X.509 Exporter](https://itnext.io/monitoring-certificates-expiration-in-kubernetes-with-x-509-exporter-8030b69f611d)

## Videos
??? note "Click to expand!"

    <center>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/5ofsNyHZwWE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </center>