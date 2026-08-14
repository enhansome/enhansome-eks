# Awesome eks with stars

![EKS logo](images/eks-logo.png)

A curated list of awesome tools for Amazon EKS 🌊

Want to add something? Open a PR! 🙂

## What is EKS

Amazon Elastic Kubernetes Service (Amazon EKS) is a managed service that makes it easy for you to run Kubernetes on AWS without needing to stand up or maintain your own Kubernetes control plane. Kubernetes is an open-source system for automating the deployment, scaling, and management of containerized applications.

Amazon EKS runs Kubernetes control plane instances across multiple Availability Zone to ensure high availability. Amazon EKS automatically detects and replaces unhealthy control plane instances, and it provides automated version upgrades and patching for them.

Amazon EKS runs up-to-date versions of the open-source Kubernetes software, so you can use all the existing plugins and tooling from the Kubernetes community. Applications running on Amazon EKS are fully compatible with applications running on any standard Kubernetes environment, whether running in on-premises data centers or public clouds. This means that you can easily migrate any standard Kubernetes application to Amazon EKS without any code modification required.

## Table of content

* [Cluster management tools](#cluster-management-tools)
* [Data plane management](#data-plane-management)
* [CLI tools](#cli-tools)
* [Package managers](#package-managers)
* [Security](#security)
* [Networking](#networking)
* [Compliance](#compliance)
* [Container runtime security](#container-runtime-security)
* [Audit](#audit)
* [Monitoring](#monitoring)
* [Logging](#logging)
* [Tracing](#tracing)
* [CI and CD tools](#ci-and-cd-tools)
* [Scaling](#pod-scaling)
* [Chaos testing](#chaos-testing)
* [Storage](#storage)
* [Ingress](#ingress)
* [API gateways](#api-gateways)
* [Service meshes](#service-meshes)
* [Backup](#backup)
* [Cost allocation](#cost-allocation)
* [Machine learning](#machine-learning)
* [Self-paced learning](#self-paced-learning)
* [Miscellaneous](#miscellaneous)
* [Upcoming Events](#upcoming-events)
* [re:Invent 2019 sessions](#re-invent-2019-sessions)
* [Twitter](#twitter)
* [Books](#books)
* [Contributors](#contributors)

***

## Cluster management tools

* [cdk8s](https://github.com/awslabs/cdk8s) ⭐ 4,849 | 🐛 77 | 🌐 JavaScript | 📅 2026-08-14 - Define Kubernetes native apps and abstractions using object-oriented programming
* [aws-k8s-tester](https://github.com/aws/aws-k8s-tester) ⭐ 184 | 🐛 11 | 🌐 Go | 📅 2026-08-09 - Implements [`k8s.io/test-infra/kubetest2`](https://github.com/kubernetes/test-infra/tree/master/kubetest2) ⭐ 4,013 | 🐛 122 | 🌐 Go | 📅 2026-08-14, creates/deletes testing EKS cluster with various add-ons.
* [ekstender](https://github.com/mreferre/ekstender) ⭐ 67 | 🐛 0 | 🌐 Shell | 📅 2020-08-11 - tool that extends a vanilla Amazon EKS cluster with a number of add-on OSS projects.
* [Octant](https://github.com/metral/octumi) ⭐ 1 | 🐛 0 | 🌐 TypeScript | 📅 2019-08-21 - Deploy VMware Octant on a EKS Cluster using Pulumi
* [eksctl](https://eksctl.io)
* [AWS CloudFormation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-eks-cluster.html)
* [CDK Amazon EKS Construct Library](https://docs.aws.amazon.com/cdk/api/latest/docs/aws-eks-readme.html)
* [Terraform](https://www.terraform.io/docs/providers/aws/guides/eks-getting-started.html)
* [Pulumi](https://www.pulumi.com/docs/tutorials/kubernetes/eks/)
* [eksctl with Ocean integration by Spot.io](https://spot.io/blog/eks-done-right-from-control-plane-to-worker-nodes/) - eksctl integrated with Ocean by Spot.io to launch EKS on spot instances with a single command

## Data plane management

* [AWS Node Termination Handler](https://github.com/aws/aws-node-termination-handler) ⭐ 1,763 | 🐛 10 | 🌐 Go | 📅 2026-07-21
* [EKS Rolling Update](https://github.com/hellofresh/eks-rolling-update) ⭐ 362 | 🐛 28 | 🌐 Python | 📅 2025-10-23
* [amazon-k8s-node-drainer](https://github.com/aws-samples/amazon-k8s-node-drainer) ⚠️ Archived
* [Managed nodes groups](https://docs.aws.amazon.com/eks/latest/userguide/managed-node-groups.html)
* [Optimized worker node management, launched on spot instances](https://eksworkshop.com/beginner/190_ocean/)

## CLI tools

* [k9s](https://github.com/derailed/k9s) ⭐ 34,349 | 🐛 115 | 🌐 Go | 📅 2026-08-14 - Provides a terminal UI to interact with your Kubernetes clusters
* [kubectx](https://github.com/ahmetb/kubectx) ⭐ 19,938 | 🐛 39 | 🌐 Go | 📅 2026-08-02 — Faster way to switch between clusters and namespaces in kubectl
* [kube-ps1](https://github.com/jonmosco/kube-ps1) ⭐ 3,806 | 🐛 5 | 🌐 Shell | 📅 2026-05-24 — Kubernetes prompt for bash and zsh.  Adds the current context and namespace to the prompt
* [kubectl tree](https://github.com/ahmetb/kubectl-tree) ⭐ 3,415 | 🐛 16 | 🌐 Go | 📅 2026-07-27
* [kui](https://github.com/IBM/kui/) ⚠️ Archived - A hybrid command-line/UI development experience for cloud-native development
* [kubectl debug](https://github.com/aylei/kubectl-debug) ⭐ 2,301 | 🐛 62 | 🌐 Go | 📅 2023-10-19 - Debug your pod by a new container with every troubleshooting tools pre-installed
* [kubectl-plugins](https://github.com/jordanwilson230/kubectl-plugins) ⭐ 636 | 🐛 16 | 🌐 Shell | 📅 2024-06-27
* [Krew](https://krew.sigs.k8s.io) - a plugin manager for kubectl

## Package managers

* [Helm](https://docs.aws.amazon.com/eks/latest/userguide/helm.html) - The Kubernetes Package Manager
* [Amazon EKS Helm chart repository](https://github.com/aws/eks-charts) ⭐ 1,302 | 🐛 222 | 🌐 Mustache | 📅 2026-08-03

## Security

* [Kyverno](https://github.com/kyverno/kyverno) ⭐ 8,032 | 🐛 585 | 🌐 Go | 📅 2026-08-14
* [kube-hunter](https://github.com/aquasecurity/kube-hunter) ⭐ 5,077 | 🐛 82 | 🌐 Python | 📅 2024-03-19
* [Gatekeeper](https://github.com/open-policy-agent/gatekeeper) ⭐ 4,263 | 🐛 172 | 🌐 Go | 📅 2026-08-10
* [Bane](https://github.com/genuinetools/bane) ⭐ 1,230 | 🐛 4 | 🌐 Go | 📅 2020-09-17 - Custom & better AppArmor profile generator for Docker containers.
* [eksuser](https://github.com/prabhatsharma/eksuser/) ⭐ 35 | 🐛 1 | 🌐 Go | 📅 2019-06-30 - Utility to manage Amazon EKS users
* [EKS Best Practices Guide for Security](https://aws.github.io/aws-eks-best-practices/)
* [Open Policy Agent](https://aws.amazon.com/blogs/opensource/using-open-policy-agent-on-amazon-eks/)
* [IAM Roles for service accounts](https://docs.aws.amazon.com/eks/latest/userguide/iam-roles-for-service-accounts.html)
* [Sysdig Falco](https://sysdig.com/blog/amazon-eks-monitoring-and-security-with-sysdig/)
* [cert-manager](https://aws.amazon.com/blogs/containers/securing-eks-ingress-contour-lets-encrypt-gitops/)
* [Pod security policy](https://docs.aws.amazon.com/eks/latest/userguide/pod-security-policy.html)

## Networking

* [ksniff](https://github.com/eldadru/ksniff) ⭐ 3,473 | 🐛 67 | 🌐 Go | 📅 2024-08-02 - Kubectl plugin to ease sniffing on kubernetes pods using tcpdump and wireshark
* [AWS VPC CNI](https://github.com/aws/amazon-vpc-cni-k8s) ⭐ 2,451 | 🐛 30 | 🌐 Go | 📅 2026-08-13
* [CNI metrics helper](https://docs.aws.amazon.com/eks/latest/userguide/cni-metrics-helper.html)
* [Calico network policy engine for Kubernetes](https://docs.aws.amazon.com/eks/latest/userguide/calico.html)
* [Cluster VPC considerations](https://docs.aws.amazon.com/eks/latest/userguide/network_reqs.html)

## Compliance

* [docker-bench-security](https://github.com/docker/docker-bench-security) ⭐ 9,686 | 🐛 29 | 🌐 Shell | 📅 2026-06-04
* [kube-bench](https://github.com/aquasecurity/kube-bench#running-in-an-eks-cluster) ⭐ 8,140 | 🐛 94 | 🌐 Go | 📅 2026-08-10
* [actuary](https://github.com/diogomonica/actuary) ⭐ 83 | 🐛 6 | 🌐 Go | 📅 2017-09-15
* [AWS Inspector](https://aws.amazon.com/inspector/)
* [Sysdig Secure](https://sysdig.com/products/kubernetes-security/)

## Container runtime security

* [Aqua](https://www.aquasec.com/products/aqua-cloud-native-security-platform/)
* [Qualys](https://www.qualys.com/apps/container-security/)
* [Amazon ECR container image scanning](https://docs.aws.amazon.com/AmazonECR/latest/userguide/image-scanning.html)
* [Twistlock](https://www.twistlock.com/2017/11/29/elastic-container-service-kubernetes-amazon-eks-twistlock/)

## Audit

* [kubeaudit](https://github.com/Shopify/kubeaudit) ⚠️ Archived
* [MKIT](https://github.com/darkbitio/mkit#example-run-against-an-eks-cluster) ⚠️ Archived
* [kaudit](https://github.com/alcideio/kaudit) ⭐ 35 | 🐛 2 | 🌐 Shell | 📅 2021-07-08
* [Logging Amazon EKS API calls with AWS CloudTrail](https://docs.aws.amazon.com/eks/latest/userguide/logging-using-cloudtrail.html)
* [kubesec.io](https://kubesec.io/)
* [polaris](https://aws.amazon.com/blogs/opensource/running-secure-workloads-eks-polaris/)

## Monitoring

* [Mizu](https://github.com/up9inc/mizu) ⭐ 12,041 | 🐛 143 | 🌐 Go | 📅 2026-08-13 - The API Traffic Viewer for Kubernetes (Think TCPDump and Wireshark re-invented for Kubernetes)
* [kube-state-metrics](https://github.com/kubernetes/kube-state-metrics) ⭐ 6,173 | 🐛 105 | 🌐 Go | 📅 2026-08-14 — Add-on agent to generate and expose cluster-level metrics.
* [k8s-image-availability-exporter](https://github.com/flant/k8s-image-availability-exporter) ⭐ 255 | 🐛 28 | 🌐 Go | 📅 2026-07-29 - Alerts if an image used in Kubernetes cannot be pulled from container registry
* [KubeStellar Console](https://github.com/kubestellar/console) ⭐ 127 | 🐛 31 | 🌐 TypeScript | 📅 2026-08-14 — Multi-cluster Kubernetes dashboard with real-time observability, AI-powered operations, and CNCF project integrations across EKS and other clusters
* [Kubernetes Metrics Server](https://docs.aws.amazon.com/eks/latest/userguide/metrics-server.html) — Cluster-wide aggregator of resource usage data
* [Prometheus + Grafana](https://eksworkshop.com/intermediate/240_monitoring/)
* [CloudWatch Container Insights](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/ContainerInsights.html)
* [Using Prometheus Metrics in Amazon CloudWatch](https://aws.amazon.com/blogs/containers/using-prometheus-metrics-in-amazon-cloudwatch/)

## Troubleshooting

* [kubespy](https://github.com/pulumi/kubespy) ⭐ 3,078 | 🐛 18 | 🌐 Go | 📅 2026-08-13
* [Sloop](https://github.com/salesforce/sloop) ⭐ 1,580 | 🐛 61 | 🌐 Go | 📅 2026-02-17

## Logging

* [Amazon EKS control plane logging](https://docs.aws.amazon.com/eks/latest/userguide/control-plane-logs.html)
* [Fluentd](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/Container-Insights-setup-logs.html) — Set Up FluentD as a DaemonSet to Send Logs to CloudWatch Logs
* [Kubernetes Logging powered by AWS for Fluent Bit](https://aws.amazon.com/blogs/containers/kubernetes-logging-powered-by-aws-for-fluent-bit/)
* [Cloudwatch Container Insights](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/Container-Insights-setup-EKS-quickstart.html)

## Tracing

* [AWS X-Ray](https://aws.amazon.com/xray/)
* [Jaeger](https://github.com/jaegertracing/jaeger) ⭐ 23,100 | 🐛 563 | 🌐 Go | 📅 2026-08-13

## CI and CD tools

* [Spinnaker](https://github.com/spinnaker/spinnaker) ⭐ 9,763 | 🐛 126 | 🌐 Java | 📅 2026-08-14
* [Flux](https://github.com/fluxcd/flux) ⚠️ Archived - The GitOps Kubernetes operator
* [Flagger](https://docs.flagger.app/install/flagger-install-on-eks-appmesh) - Progressive Delivery Operator for Kubernetes
* Jenkins
* [Jenkins X](https://docs.cloudbees.com/docs/cloudbees-jenkins-x-distribution/latest/eks-install-guide/eks-boot)
* Travis
* [Circle CI](https://circleci.com/integrations/kubernetes/)
* [Gitlab](https://docs.gitlab.com/ee/user/project/clusters/add_eks_clusters.html)
* [Shippable](http://docs.shippable.com/getting-started/tutorials/)
* [Argo](https://eksworkshop.com/advanced/410_batch/deploy/)

## Pod scaling

* [Goldilocks vertical-pod-autoscaler](https://github.com/FairwindsOps/goldilocks/) ⭐ 3,314 | 🐛 13 | 🌐 Go | 📅 2026-08-14
* [Escalator](https://github.com/atlassian/escalator) ⭐ 686 | 🐛 18 | 🌐 Go | 📅 2026-07-06 - A batch or job optimized horizontal autoscaler
* [kube-metrics-adapter](https://github.com/zalando-incubator/kube-metrics-adapter) ⭐ 543 | 🐛 12 | 🌐 Go | 📅 2026-08-13
* [right-size-guide](https://github.com/mhausenblas/right-size-guide) ⭐ 57 | 🐛 1 | 🌐 Go | 📅 2020-03-26 — A CLI tool providing memory & CPU recommendations for containerized apps
* [Automatic right-sizing](https://spot.io/blog/kubernetes-automatic-rightsizing-with-dynamic-admission-controller/) — Using Kubernetes [dynamic admission controller](https://kubernetes.io/docs/reference/access-authn-authz/extensible-admission-controllers/) to implement automatic right-sizing recommendations

## Chaos testing

* [Chaos Mesh](https://github.com/pingcap/chaos-mesh) ⭐ 7,843 | 🐛 542 | 🌐 Go | 📅 2026-08-07
* [LitmusChaos](https://github.com/litmuschaos/litmus) ⭐ 5,595 | 🐛 414 | 🌐 Go | 📅 2026-07-31
* [kube-monkey](https://github.com/asobti/kube-monkey) ⭐ 3,063 | 🐛 25 | 🌐 Go | 📅 2026-08-12
* [PowerfulSeal](https://github.com/bloomberg/powerfulseal) ⭐ 1,976 | 🐛 55 | 🌐 Python | 📅 2023-11-10
* [chaoskube](https://github.com/linki/chaoskube) ⭐ 1,934 | 🐛 34 | 🌐 Go | 📅 2026-08-01
* [Gremlin](https://www.gremlin.com/community/tutorials/how-to-install-and-use-gremlin-with-eks/)

## Storage

* [Rook](https://github.com/rook/rook) ⭐ 13,596 | 🐛 127 | 🌐 Go | 📅 2026-08-14
* [Amazon EBS CSI driver](https://github.com/kubernetes-sigs/aws-ebs-csi-driver) ⭐ 1,134 | 🐛 27 | 🌐 Go | 📅 2026-08-05
* [Amazon EFS CSI driver](https://github.com/kubernetes-sigs/aws-efs-csi-driver) ⭐ 804 | 🐛 12 | 🌐 Go | 📅 2026-08-03
* [Amazon FSx for Lustre CSI driver](https://github.com/kubernetes-sigs/aws-fsx-csi-driver) ⭐ 144 | 🐛 11 | 🌐 Go | 📅 2026-08-05
* [OpenEBS](https://help.mayadata.io/hc/en-us/articles/360037226451-Creating-an-OpenEBS-cluster-in-an-EKS-cluster)

## Ingress

* [ALB Ingress Controller](https://github.com/kubernetes-sigs/aws-alb-ingress-controller) ⭐ 4,319 | 🐛 128 | 🌐 Go | 📅 2026-08-13 - AWS ALB Ingress Controller for Kubernetes
* [Contour](https://github.com/projectcontour/contour) ⭐ 3,943 | 🐛 121 | 🌐 HTML | 📅 2026-08-12
* [Gloo](https://github.com/solo-io/gloo) ⭐ 169 | 🐛 1,862 | 🌐 Go | 📅 2026-08-13 - The Feature-rich, Kubernetes-native, Next-Generation API Gateway Built on Envoy
* [Traefik](https://containo.us/traefik/) — Cloud Native Edge Router
* [Nginx](https://aws.amazon.com/blogs/opensource/network-load-balancer-nginx-ingress-controller-eks/)

## API gateways

* [Kong](https://github.com/Kong/kong) ⭐ 43,983 | 🐛 188 | 🌐 Lua | 📅 2026-08-04
* [Ambassador](https://github.com/datawire/ambassador) ⭐ 4,518 | 🐛 441 | 🌐 Python | 📅 2026-08-13
* [Amazon API Gateway](https://aws.amazon.com/blogs/containers/api-gateway-as-an-ingress-controller-for-eks/)

## Service meshes

* [AppMesh](https://docs.aws.amazon.com/eks/latest/userguide/appmesh-getting-started.html)
* [Istio](https://aws.amazon.com/blogs/opensource/getting-started-istio-eks/)
* [Linkerd](http://linkerd.io)
* [Consul](https://learn.hashicorp.com/consul/kubernetes/aws-k8s)

## Backup

* [Velero](https://eksworkshop.com/intermediate/280_backup-and-restore/)
* [Kasten K10](https://kasten.io)

## Cost allocation

* [kubecost](https://kubecost.com)
* [Kubernetes Opex Analytics](https://github.com/rchakode/kube-opex-analytics) ⭐ 484 | 🐛 9 | 🌐 Python | 📅 2026-07-31
* [Kubernetes Cost Allocation](https://spot.io/blog/kubernetes-workload-chargeback-and-showback/)

## Machine learning

* [Kubeflow](https://github.com/kubeflow/kubeflow) ⭐ 15,813 | 🐛 0 | 📅 2026-07-10 — Machine Learning Toolkit for Kubernetes
* [Optimizing Spark performance on Kubernetes](https://aws.amazon.com/blogs/containers/optimizing-spark-performance-on-kubernetes/)
* [**Video** AWS re:Invent 2019: Building machine-learning infrastructure on Amazon EKS with Kubeflow (CON306-R1)](https://www.youtube.com/watch?v=ULlqukKVKBo)

## Self-paced learning

* [EKS Workshop](https://eksworkshop.com)
* [Amazon EKS and Kubernetes on EC2 Container Networking Workshop](https://awsk8snetworkshops.com/)
* [AWS Kubeflow Workshop](https://master.d2j834wqg8s4j0.amplifyapp.com/)
* [App Mesh Workshop](https://www.appmeshworkshop.com/)
* [Blue Green Deployment with Amazon EKS and K8s](https://awsdemoworkshops.s3.us-east-2.amazonaws.com/cicd-eks-alb-bg-cdk-workshop/public/en/index.html)
* [EKS/ECR/ECS Modernization](https://modernize.awsworkshop.io)
* [GitOps Helm Workshop](https://helm.workshop.flagger.dev/)
* [Introduction to GitOps on Amazon EKS with Weaveworks](https://weaveworks-gitops.awsworkshop.io/)

## Miscellaneous

* [AWS container services roadmap](https://github.com/aws/containers-roadmap/projects/1) ⭐ 5,357 | 🐛 1,597 | 🌐 Shell | 📅 2025-03-25
* [Container content ideas for AWS](https://github.com/awslabs/container-content-ideas-for-aws/projects/1) ⚠️ Archived
* [AWS containers blog](https://aws.amazon.com/blogs/containers/)
* [Nick Brandaleone's blog](https://www.nickaws.net)
* [Amazon EKS Kubernetes versions](https://docs.aws.amazon.com/eks/latest/userguide/kubernetes-versions.html#kubernetes-1.16)
* [Windows support](https://docs.aws.amazon.com/eks/latest/userguide/windows-support.html)
* [ARM Support](https://docs.aws.amazon.com/eks/latest/userguide/arm-support.html)
* [Amazon EKS on AWS Outposts](https://docs.aws.amazon.com/eks/latest/userguide/eks-on-outposts.html)
* [Awesome AWS Workshops](https://awesome-aws-workshops.com/#containers)

## Upcoming events

* July 9, 2020 - [AWS Cloud Containers Conference](https://awscloudcontainersconference.splashthat.com/?\&trk=el_a134p000003yOg3AAE\&trkCampaign=AWS_Cloud_Containers_Conference\&sc_channel=el\&sc_campaign=GLOBAL_PM_WEBINAR_aws-cloud-containers-conference_20200709\&sc_outcome=Product_Marketing\&sc_geo=mult)

## re:Invent 2019 sessions

* [AWS re:Invent 2019: Running Kubernetes at Amazon scale using Amazon EKS (CON212-R1)](https://www.youtube.com/watch?v=M-Fh0OzliJI)
* [AWS re:Invent 2019: Running Kubernetes Applications on AWS Fargate (CON326-R1)](https://www.youtube.com/watch?v=m-3tMXmWWQw)
* [AWS re:Invent 2019: Amazon EKS under the hood (CON421-R1)](https://www.youtube.com/watch?v=7vxDWDD2YnM)
* [AWS re:Invent 2019: Building machine-learning infrastructure on Amazon EKS with Kubeflow (CON306-R1)](https://www.youtube.com/watch?v=ULlqukKVKBo)
* [AWS re:Invent 2019: How Ticketmaster runs Kubernetes for 80% less without managing VMs (CON308-S)](https://www.youtube.com/watch?v=X7RmfleuWrw)

## Twitter

* [Chris Short](https://twitter.com/ChrisShort) - AWS Developer Advocate
* [Massimo Re Ferre'](https://twitter.com/mreferre) - AWS Developer Advocate
* [Michael Hausenblas](https://twitter.com/mhausenblas) - AWS Developer Advocate

## Books

* Container Security by Liz Rice
* Kubernetes Patterns by Roland Huß
* Kubernetes Best Practices by Lachlan Evenson, Dave Strebel, Eddie Villalba, Brendan Burns
* Programming Kubernetes by Michael Hausenblas and Stefan Schimanski
* Kubernetes Cookbook by Sébastien Goasguen and Michael Hausenblas
* Mastering Kubernetes by Gigi Sayfan
* Kubernetes Security by Liz Rice and Michael Hausenblas
* Kubernetes - A Complete DevOps Cookbook by Murat Karslioglu

## Maintainers

[@realvz](https://twitter.com/realz)

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-14._
