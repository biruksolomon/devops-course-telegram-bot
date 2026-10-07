# DevOps Course: Curriculum

A beginner-to-job-ready DevOps course delivered on Telegram: **111 lessons**, **4 lessons per day**, about **28 days**.

Posting times (set in the n8n Schedule Trigger): 08:00, 12:00, 16:00, 20:00.

## Modules

| # | Module | Lessons | Lesson numbers | Days |
|---|--------|---------|----------------|------|
| 1 | DevOps basics and mindset | 4 | 1-4 | 1-1 |
| 2 | Linux essentials | 10 | 5-14 | 2-4 |
| 3 | Networking basics | 6 | 15-20 | 4-5 |
| 4 | Git and GitHub | 8 | 21-28 | 6-7 |
| 5 | Bash scripting | 6 | 29-34 | 8-9 |
| 6 | Docker | 12 | 35-46 | 9-12 |
| 7 | Docker Compose | 5 | 47-51 | 12-13 |
| 8 | CI/CD with GitHub Actions | 8 | 52-59 | 13-15 |
| 9 | Cloud basics with AWS | 10 | 60-69 | 15-18 |
| 10 | Infrastructure as Code with Terraform | 8 | 70-77 | 18-20 |
| 11 | Configuration management with Ansible | 5 | 78-82 | 20-21 |
| 12 | Kubernetes | 14 | 83-96 | 21-24 |
| 13 | Monitoring and logging | 6 | 97-102 | 25-26 |
| 14 | DevSecOps | 5 | 103-107 | 26-27 |
| 15 | Capstone project | 4 | 108-111 | 27-28 |
| | **Total** | **111** | 1-111 | **28** |

## Every lesson follows the same format

1. Title with lesson number
2. Short explanation in simple words
3. A real-world analogy
4. A tested example (commands or config) in a code block
5. One small practice task
6. A one-line teaser for the next lesson

Each lesson is written by AI from the topic and key points below, then reviewed by a human before it is posted. It must stay under 4096 characters (the Telegram limit).

## Full lesson list


### DevOps basics and mindset

| Lesson | Day | Time | Topic | Key points |
|--------|-----|------|-------|------------|
| 1 | 1 | 08:00 | What is DevOps? | Dev and Ops silos before DevOps; culture + practices + tools; goals: faster and safer delivery |
| 2 | 1 | 12:00 | The DevOps lifecycle | plan, code, build, test, release, deploy, operate, monitor; the feedback loop |
| 3 | 1 | 16:00 | Core DevOps practices | CI, CD, infrastructure as code, monitoring, collaboration; why small frequent releases are safer |
| 4 | 1 | 20:00 | DevOps roles, tools and the learning roadmap | DevOps engineer vs SRE vs platform engineer; tool map of this course; how to practice every day |

### Linux essentials

| Lesson | Day | Time | Topic | Key points |
|--------|-----|------|-------|------------|
| 5 | 2 | 08:00 | Why Linux and setting up a practice machine | Linux on servers, cloud and containers; options: Ubuntu, WSL, virtual machine; open a terminal |
| 6 | 2 | 12:00 | The terminal and basic navigation | pwd, ls, cd; absolute vs relative paths; tab completion; man and --help |
| 7 | 2 | 16:00 | Files and directories | mkdir, touch, cp, mv, rm; wildcards; danger of rm -rf |
| 8 | 2 | 20:00 | Viewing and searching files | cat, less, head, tail -f, wc; grep basics |
| 9 | 3 | 08:00 | The Linux directory structure | /, /etc, /var, /home, /usr, /tmp, /bin; where configs and logs live |
| 10 | 3 | 12:00 | Users, groups and sudo | whoami, adduser, usermod, groups; sudo vs root; least privilege |
| 11 | 3 | 16:00 | File permissions | reading ls -l; rwx for user/group/other; chmod numeric and symbolic; chown |
| 12 | 3 | 20:00 | Processes and services | ps, top, kill; systemctl status/start/stop/enable; journalctl for logs |
| 13 | 4 | 08:00 | Package management | apt update, install, remove; repositories; why we update; dnf mention |
| 14 | 4 | 12:00 | Pipes, redirection and environment variables | |, >, >>, 2>; export; PATH; .bashrc |

### Networking basics

| Lesson | Day | Time | Topic | Key points |
|--------|-----|------|-------|------------|
| 15 | 4 | 16:00 | IP addresses, DNS and ports | what an IP address is; DNS name resolution; common ports 22, 80, 443 |
| 16 | 4 | 20:00 | TCP, UDP and HTTP | TCP vs UDP; HTTP methods and status codes; HTTPS and TLS in simple terms |
| 17 | 5 | 08:00 | Networking commands you will use daily | ping, curl, dig, ss -tulpn, ip addr, traceroute |
| 18 | 5 | 12:00 | SSH: connecting to servers | ssh user@host; ssh-keygen key pairs; authorized_keys; never share the private key |
| 19 | 5 | 16:00 | Firewalls and open ports | ufw: default deny, allow 22/80/443; why open the minimum ports |
| 20 | 5 | 20:00 | Reverse proxies and load balancers | forward vs reverse proxy; Nginx role; load balancing idea; TLS termination |

### Git and GitHub

| Lesson | Day | Time | Topic | Key points |
|--------|-----|------|-------|------------|
| 21 | 6 | 08:00 | What is version control? | history and collaboration; Git vs GitHub; install Git; git config user.name and user.email |
| 22 | 6 | 12:00 | Your first repository | git init, status, add, commit, log; writing good commit messages |
| 23 | 6 | 16:00 | Branching and merging | git branch, switch -c, merge; fast-forward vs merge commit |
| 24 | 6 | 20:00 | Remote repositories | git remote add, push, pull, clone; authenticating with SSH key or token |
| 25 | 7 | 08:00 | Resolving merge conflicts | what conflict markers look like; edit, add, commit; how to avoid conflicts |
| 26 | 7 | 12:00 | Pull requests and code review | branch, push, open a PR; reviews; protected branches |
| 27 | 7 | 16:00 | Undoing changes safely | git restore, reset (soft, mixed, hard), revert, commit --amend; never rewrite pushed history |
| 28 | 7 | 20:00 | Git workflows and .gitignore | trunk-based vs GitFlow; .gitignore; tags; never commit secrets |

### Bash scripting

| Lesson | Day | Time | Topic | Key points |
|--------|-----|------|-------|------------|
| 29 | 8 | 08:00 | Your first Bash script | shebang line; chmod +x; run it; echo |
| 30 | 8 | 12:00 | Variables, arguments and input | variables; $1 and $@; read; quoting; command substitution |
| 31 | 8 | 16:00 | Conditions and loops | if/elif/else with [[ ]]; for and while; exit codes and $? |
| 32 | 8 | 20:00 | Functions and error handling | functions; set -euo pipefail; trap; meaningful exit codes |
| 33 | 9 | 08:00 | Useful automation scripts | backup script; log cleanup; simple health check |
| 34 | 9 | 12:00 | Scheduling with cron | crontab -e; five time fields; use absolute paths; checking cron logs |

### Docker

| Lesson | Day | Time | Topic | Key points |
|--------|-----|------|-------|------------|
| 35 | 9 | 16:00 | What is Docker and why containers? | containers vs virtual machines; image vs container; the works-on-my-machine problem |
| 36 | 9 | 20:00 | Installing Docker and running hello-world | install on Ubuntu; docker version; docker run hello-world; what happens behind the scenes |
| 37 | 10 | 08:00 | Working with images | docker pull, images, rmi; tags; Docker Hub; official images |
| 38 | 10 | 12:00 | Running containers | docker run -d -p; ps; stop; rm; logs; exec -it |
| 39 | 10 | 16:00 | Your first Dockerfile | FROM, WORKDIR, COPY, RUN, CMD; docker build -t; run your image |
| 40 | 10 | 20:00 | Dockerfile best practices | layer caching; .dockerignore; small base images; running as non-root user |
| 41 | 11 | 08:00 | Docker volumes and bind mounts | why container data disappears; named volumes; bind mounts; -v flag |
| 42 | 11 | 12:00 | Docker networking | bridge network; user-defined networks; container-name DNS; publishing ports |
| 43 | 11 | 16:00 | Environment variables and configuration | -e and --env-file; configuration vs code; never bake secrets into images |
| 44 | 11 | 20:00 | Multi-stage builds | build stage and runtime stage; example: Maven build of a Spring Boot jar into a small JRE image |
| 45 | 12 | 08:00 | Docker registries | docker tag; docker login; push to Docker Hub or GHCR; pull on another machine |
| 46 | 12 | 12:00 | Docker troubleshooting and cleanup | logs; inspect; exec; common errors; docker system prune carefully |

### Docker Compose

| Lesson | Day | Time | Topic | Key points |
|--------|-----|------|-------|------------|
| 47 | 12 | 16:00 | Why Docker Compose? | problems with many docker run commands; services in one YAML file; docker compose up and down |
| 48 | 12 | 20:00 | Writing a compose file | services; image; ports; environment; volumes; running and stopping |
| 49 | 13 | 08:00 | Compose networking and dependencies | default network; service names as hostnames; depends_on with healthcheck |
| 50 | 13 | 12:00 | A multi-service app: API and PostgreSQL | app + database + named volume; connection string using the service name |
| 51 | 13 | 16:00 | Compose in practice | logs; build; .env file; override files; profiles |

### CI/CD with GitHub Actions

| Lesson | Day | Time | Topic | Key points |
|--------|-----|------|-------|------------|
| 52 | 13 | 20:00 | What are CI and CD? | continuous integration, delivery and deployment; pipeline stages; benefits and risks |
| 53 | 14 | 08:00 | GitHub Actions concepts | workflow, event, job, step, runner, action; the .github/workflows folder |
| 54 | 14 | 12:00 | Your first workflow | on: push; runs-on ubuntu-latest; actions/checkout; run steps; reading the logs |
| 55 | 14 | 16:00 | Building and testing code | setup-java; mvn test; fail the pipeline on failing tests; matrix builds idea |
| 56 | 14 | 20:00 | Caching and artifacts | actions/cache to speed up builds; upload-artifact and download-artifact |
| 57 | 15 | 08:00 | Secrets and environment variables | repository secrets; secrets context; never print secrets; environments |
| 58 | 15 | 12:00 | Building and pushing Docker images in CI | docker/login-action; build-push-action; push to GHCR or Docker Hub; tags |
| 59 | 15 | 16:00 | Deploying from a pipeline | deploy over SSH or to the cloud; manual approvals; rollback idea; deployment safety |

### Cloud basics with AWS

| Lesson | Day | Time | Topic | Key points |
|--------|-----|------|-------|------------|
| 60 | 15 | 20:00 | What is cloud computing? | IaaS, PaaS, SaaS; regions and availability zones; pay-as-you-go; shared responsibility model |
| 61 | 16 | 08:00 | Creating an AWS account safely | free tier; MFA on the root account; budget alerts; create an IAM admin user |
| 62 | 16 | 12:00 | IAM: users, roles and policies | least privilege; policy JSON basics; roles vs users; never use root for daily work |
| 63 | 16 | 16:00 | EC2: virtual servers | AMI; instance types; key pair; launch and connect by SSH; stop vs terminate |
| 64 | 16 | 20:00 | VPC and security groups | VPC; public and private subnets; internet gateway; security groups as firewalls |
| 65 | 17 | 08:00 | S3: object storage | buckets and objects; block public access; versioning; common use cases |
| 66 | 17 | 12:00 | EBS storage and snapshots | block storage vs object storage; attach a volume; snapshots for backup |
| 67 | 17 | 16:00 | RDS: managed databases | managed vs self-hosted; backups; Multi-AZ; protect with security groups |
| 68 | 17 | 20:00 | Load balancing and auto scaling | application load balancer; target groups; health checks; auto scaling groups |
| 69 | 18 | 08:00 | Cloud cost control | budgets; tagging; stop unused resources; free tier traps |

### Infrastructure as Code with Terraform

| Lesson | Day | Time | Topic | Key points |
|--------|-----|------|-------|------------|
| 70 | 18 | 12:00 | What is Infrastructure as Code? | declarative vs imperative; benefits; Terraform vs CloudFormation |
| 71 | 18 | 16:00 | Installing Terraform and the core workflow | init, plan, apply, destroy; providers |
| 72 | 18 | 20:00 | Your first resource: an S3 bucket | provider block; resource block; authenticate via environment or aws configure; apply and destroy |
| 73 | 19 | 08:00 | Variables, outputs and locals | variable blocks; terraform.tfvars; outputs; locals |
| 74 | 19 | 12:00 | State and remote backends | what terraform.tfstate holds; why never commit it; remote state with locking |
| 75 | 19 | 16:00 | Building an EC2 server with Terraform | aws_instance; security group; data source for the AMI; output the public IP |
| 76 | 19 | 20:00 | Terraform modules | reuse; module inputs and outputs; registry modules; folder structure |
| 77 | 20 | 08:00 | Terraform best practices | fmt and validate; workspaces; plan on pull requests; handling secrets |

### Configuration management with Ansible

| Lesson | Day | Time | Topic | Key points |
|--------|-----|------|-------|------------|
| 78 | 20 | 12:00 | What is configuration management? | agentless over SSH; idempotency; Terraform vs Ansible |
| 79 | 20 | 16:00 | Inventory and ad-hoc commands | inventory file; ansible all -m ping; running ad-hoc commands |
| 80 | 20 | 20:00 | Your first playbook | YAML basics; hosts and tasks; the apt module; ansible-playbook |
| 81 | 21 | 08:00 | Variables, handlers and templates | vars; notify and handlers; Jinja2 templates |
| 82 | 21 | 12:00 | Roles and Ansible Vault | role folder structure; ansible-galaxy init; encrypting secrets with Vault |

### Kubernetes

| Lesson | Day | Time | Topic | Key points |
|--------|-----|------|-------|------------|
| 83 | 21 | 16:00 | Why Kubernetes? | problems it solves: scaling, self-healing, rollouts; when you do not need it |
| 84 | 21 | 20:00 | Kubernetes architecture | control plane: API server, etcd, scheduler, controller manager; nodes: kubelet, kube-proxy, runtime |
| 85 | 22 | 08:00 | Setting up a local cluster | minikube or kind; install kubectl; kubectl get nodes |
| 86 | 22 | 12:00 | Pods | the smallest unit; pod YAML; kubectl apply, get, describe, delete |
| 87 | 22 | 16:00 | Deployments and ReplicaSets | desired replicas; self-healing; kubectl scale |
| 88 | 22 | 20:00 | Services | ClusterIP, NodePort, LoadBalancer; labels and selectors |
| 89 | 23 | 08:00 | Rolling updates and rollbacks | kubectl set image; rollout status; rollout undo; update strategy |
| 90 | 23 | 12:00 | ConfigMaps and Secrets | injecting configuration; env vars vs mounted files; Secrets are base64, not encryption |
| 91 | 23 | 16:00 | Persistent storage | PersistentVolume; PersistentVolumeClaim; StorageClass; stateful data |
| 92 | 23 | 20:00 | Ingress | HTTP routing by host and path; ingress controller; nginx ingress example |
| 93 | 24 | 08:00 | Namespaces, requests and limits | namespaces; resource requests and limits; what OOMKilled means |
| 94 | 24 | 12:00 | Health probes | liveness, readiness and startup probes; when each one restarts or removes a pod |
| 95 | 24 | 16:00 | Helm | charts; values.yaml; helm install, upgrade, rollback |
| 96 | 24 | 20:00 | Debugging Kubernetes | logs; describe; events; exec; CrashLoopBackOff; ImagePullBackOff |

### Monitoring and logging

| Lesson | Day | Time | Topic | Key points |
|--------|-----|------|-------|------------|
| 97 | 25 | 08:00 | Why monitoring and observability? | metrics, logs, traces; SLIs and SLOs; why alerts matter |
| 98 | 25 | 12:00 | Prometheus basics | scraping; metric types; exporters; first PromQL queries |
| 99 | 25 | 16:00 | Grafana dashboards | add a data source; panels; build a simple dashboard |
| 100 | 25 | 20:00 | Alerting | Alertmanager; writing useful alerts; avoiding alert fatigue; sending alerts to Telegram |
| 101 | 26 | 08:00 | Centralized logging | why central logs; Loki and ELK overview; structured logs |
| 102 | 26 | 12:00 | Incident response and postmortems | on-call; runbooks; blameless postmortems |

### DevSecOps

| Lesson | Day | Time | Topic | Key points |
|--------|-----|------|-------|------------|
| 103 | 26 | 16:00 | What is DevSecOps? | shift security left; threat basics; secure development lifecycle |
| 104 | 26 | 20:00 | Secrets management | never in Git; environment variables; vaults; rotation; secret scanning |
| 105 | 27 | 08:00 | Container and image security | minimal base images; non-root; scanning with Trivy; pin versions |
| 106 | 27 | 12:00 | Dependency and code scanning | Dependabot; SAST and CodeQL; reading scan results |
| 107 | 27 | 16:00 | Hardening servers and cloud access | SSH hardening; MFA; least privilege; patching; audit logs |

### Capstone project

| Lesson | Day | Time | Topic | Key points |
|--------|-----|------|-------|------------|
| 108 | 27 | 20:00 | Capstone: plan the project | choose a simple Spring Boot API; draw the architecture; write a requirements checklist |
| 109 | 28 | 08:00 | Capstone: containerize and add CI | Dockerfile; Compose file; GitHub Actions build and test pipeline |
| 110 | 28 | 12:00 | Capstone: deploy the infrastructure and app | Terraform EC2 server; deploy the container; basic HTTPS |
| 111 | 28 | 16:00 | Capstone: monitor, document and next steps | add monitoring; write the README; portfolio tips; career roadmap |
