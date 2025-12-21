# ☸️ KUBERNETES SKILLS - Scored Recommendations

## Category: Kubernetes Orchestration & Cluster Management

---

## 📊 COMPREHENSIVE SCORING

| Repository | Overall | Functionality | Flexibility | Portability | Docs | License | Active |
|------------|---------|---------------|-------------|-------------|------|---------|--------|
| **wshobson/agents** | **9.3** | 10 | 10 | 9 | 9 | 10 | 9 |
| **ahmedasmar/devops-claude-skills** | **9.0** | 9 | 9 | 9 | 9 | 10 | 9 |
| **mrgoonie/claudekit-skills** | **7.5** | 7 | 8 | 8 | 7 | 10 | 9 |

**Scoring Criteria (1-10):**
- **Functionality:** Features, capabilities, K8s coverage
- **Flexibility:** Modularity, customization, adaptability
- **Portability:** Cross-platform, git-friendly, dependencies
- **Documentation:** Quality, completeness, examples
- **License:** Permissiveness (10=MIT/Apache, 5=restrictive)
- **Active:** Maintenance, updates, community support

---

## 🥇 BEST: wshobson/agents
**Overall Score: 9.3/10**

### Strengths
✓ **Most comprehensive** - 107 specialized skills across 18 plugins
✓ **Production-grade K8s configs** - Enterprise-ready manifests
✓ **Multi-agent orchestration** - Specialized agents for different tasks
✓ **Kubernetes-architect agent** - 4 specialized K8s skills
✓ **Progressive disclosure** - Minimal context usage (efficient)
✓ **Modular architecture** - 3.4 components per plugin average
✓ **Helm chart expertise** - Advanced chart development
✓ **Security-first** - Policy configuration built-in
✓ **GitOps ready** - ArgoCD, Flux patterns

### Capabilities

**kubernetes-operations Plugin (4 Skills):**
1. **Manifest Generation**
   - Deployments, Services, ConfigMaps, Secrets
   - StatefulSets, DaemonSets, Jobs, CronJobs
   - Ingress, NetworkPolicy, PersistentVolumeClaims
   - Best practices enforcement
   - YAML validation
   - Resource optimization

2. **Helm Chart Development**
   - Chart scaffolding
   - Template creation
   - Values.yaml optimization
   - Chart testing
   - Dependency management
   - Version management

3. **GitOps Deployment Patterns**
   - ArgoCD application definitions
   - Flux CD configurations
   - Multi-cluster deployments
   - Progressive delivery
   - Automated rollbacks
   - Sync policies

4. **Security Policy Configuration**
   - Pod Security Standards
   - Network policies
   - RBAC configurations
   - Security contexts
   - OPA/Gatekeeper policies
   - Secret management

**kubernetes-architect Agent:**
- Production-grade configurations
- Multi-cluster strategies
- High availability patterns
- Disaster recovery planning
- Performance optimization
- Cost optimization

### Installation
```bash
# Method 1: Via Claude Code plugin system
/plugin install kubernetes-operations

# Method 2: Manual installation
git clone https://github.com/wshobson/agents.git
cp -r agents/plugins/kubernetes-operations ~/.claude/skills/

# Verify installation
ls ~/.claude/skills/kubernetes-operations/
```

### Use Cases
- ✓ Generating production-ready K8s manifests
- ✓ Creating Helm charts from scratch
- ✓ Implementing GitOps workflows
- ✓ Configuring security policies
- ✓ Multi-cluster deployments
- ✓ K8s architecture design
- ✓ Migration planning
- ✓ Performance tuning

### Scoring Breakdown
| Metric | Score | Rationale |
|--------|-------|-----------|
| Functionality | 10/10 | Most comprehensive K8s coverage |
| Flexibility | 10/10 | Highly modular, multi-agent design |
| Portability | 9/10 | Git-friendly, minimal dependencies |
| Documentation | 9/10 | Excellent skill descriptions |
| License | 10/10 | Open source |
| Active Development | 9/10 | Regular updates, active community |

### Platform Support
- **Linux Desktop:** ✓✓✓ Full support
- **macOS:** ✓✓✓ Full support
- **Windows:** ✓✓ WSL2 recommended
- **Android Native:** ✗ Not supported
- **Android Remote:** ✓ SSH access, kubectl from phone

### Dependencies
- **Required:** None (generates configs only)
- **Optional for deployment:**
  - kubectl CLI
  - Helm 3+
  - ArgoCD/Flux (for GitOps)
  - Access to K8s cluster

### Example Usage
```bash
# In Claude Code, ask:
"Create a production-ready deployment for a Node.js app with:
- 3 replicas
- Health checks
- Resource limits
- ConfigMap for environment variables
- Horizontal Pod Autoscaler
- Network policy for security"

# Claude will use kubernetes-operations plugin to generate
# all necessary manifests with best practices
```

---

## 🥈 ALTERNATIVE 1: ahmedasmar/devops-claude-skills
**Overall Score: 9.0/10**

### Strengths
✓ **Best K8s troubleshooting** - Systematic diagnostics playbooks
✓ **Incident response focus** - 60-80% faster resolution
✓ **Production battle-tested** - Real-world scenarios
✓ **GitOps workflows** - ArgoCD and Flux expertise
✓ **Monitoring integration** - Observability patterns
✓ **MIT license** - Most permissive
✓ **Active maintenance** - Regular updates
✓ **CI/CD integration** - Pipeline patterns for K8s

### Capabilities

**k8s-troubleshooter Skill:**
- Cluster diagnostics
  - Node health checks
  - Pod crash analysis
  - Resource exhaustion detection
  - Network connectivity issues
  - Storage problems
  - Certificate expiration

- Incident response playbooks
  - Pod stuck in Pending
  - CrashLoopBackOff resolution
  - ImagePullBackOff fixes
  - OOMKilled investigation
  - Node NotReady troubleshooting
  - Service discovery issues

- Performance optimization
  - Resource requests/limits tuning
  - HPA configuration
  - Cluster autoscaling
  - Network performance
  - Storage optimization

**gitops-workflows Skill:**
- ArgoCD implementation
  - Application definitions
  - Multi-cluster setup
  - Sync policies
  - Automated rollbacks

- Flux CD deployment
  - GitRepository sources
  - Kustomization
  - Helm releases
  - Image automation

- Secrets management
  - Sealed Secrets
  - External Secrets Operator
  - Vault integration
  - SOPS encryption

**monitoring-observability Skill:**
- Prometheus setup
- Grafana dashboards
- Distributed tracing
- SLO/SLA calculation
- Alerting strategies

### Installation
```bash
# Add marketplace
/plugin marketplace add https://github.com/ahmedasmar/devops-claude-skills

# Install specific skills
/plugin install k8s-troubleshooter@devops-skills
/plugin install gitops-workflows@devops-skills
/plugin install monitoring-observability@devops-skills

# Or manual installation
git clone https://github.com/ahmedasmar/devops-claude-skills.git
cp -r devops-claude-skills/k8s-troubleshooter ~/.claude/skills/
cp -r devops-claude-skills/gitops-workflows ~/.claude/skills/
```

### Use Cases
- ✓ Troubleshooting production K8s issues
- ✓ Incident response automation
- ✓ GitOps implementation
- ✓ Monitoring and observability
- ✓ Performance optimization
- ✓ Cost optimization
- ✓ Security hardening

### Scoring Breakdown
| Metric | Score | Rationale |
|--------|-------|-----------|
| Functionality | 9/10 | Excellent troubleshooting + GitOps |
| Flexibility | 9/10 | Modular, cloud-agnostic |
| Portability | 9/10 | Python-based, minimal deps |
| Documentation | 9/10 | Clear playbooks, examples |
| License | 10/10 | MIT (most permissive) |
| Active Development | 9/10 | Active, responsive |

### Platform Support
- **Linux Desktop:** ✓✓✓ Full support
- **macOS:** ✓✓✓ Full support
- **Windows:** ✓✓ PowerShell/WSL2
- **Android Native:** ✗ Not supported
- **Android Remote:** ✓ SSH + kubectl, web dashboards

### Dependencies
- Python 3.8+ (99.6% of codebase)
- kubectl CLI (for cluster access)
- Cloud CLI tools (AWS, GCP) - optional
- Terraform - optional (for IaC skill)

---

## 🥉 ALTERNATIVE 2: mrgoonie/claudekit-skills
**Overall Score: 7.5/10**

### Strengths
✓ **Multi-cloud focus** - GCP + Kubernetes integration
✓ **DevOps skill** - Broader than just K8s
✓ **Active development** - Very frequent updates
✓ **Backend integration** - Containerized services
✓ **Cloud-native design** - Good for cloud deployments
✓ **Serverless + K8s hybrid** - Modern architectures

### Capabilities

**devops Skill:**
- Google Cloud Platform
  - GKE (Google Kubernetes Engine) deployment
  - Cloud Run + K8s hybrid
  - GCP networking with K8s
  - IAM integration

- Kubernetes deployment
  - Basic manifest generation
  - Service deployment
  - ConfigMap/Secret management
  - Ingress configuration

- CI/CD pipelines
  - Cloud Build + K8s
  - GitHub Actions for K8s
  - Automated deployments

- Container orchestration
  - Docker + K8s integration
  - Multi-container applications
  - Service mesh basics

### Installation
```bash
# Clone repository
git clone https://github.com/mrgoonie/claudekit-skills.git

# Install DevOps skill
cp -r claudekit-skills/devops ~/.claude/skills/claudekit-devops

# Verify
ls ~/.claude/skills/claudekit-devops/
```

### Use Cases
- ✓ GKE deployments
- ✓ Multi-cloud K8s
- ✓ Cloud-native applications
- ✓ Serverless + K8s hybrid
- ✓ Containerized microservices

### Scoring Breakdown
| Metric | Score | Rationale |
|--------|-------|-----------|
| Functionality | 7/10 | Good K8s basics, GCP focus |
| Flexibility | 8/10 | Multi-cloud, adaptable |
| Portability | 8/10 | Python-based, cloud deps |
| Documentation | 7/10 | Good but could be more detailed |
| License | 10/10 | Open source |
| Active Development | 9/10 | Very active updates |

### Platform Support
- **Linux Desktop:** ✓✓✓ Full support
- **macOS:** ✓✓✓ Full support
- **Windows:** ✓✓ WSL2 recommended
- **Android Native:** ✗ Not supported
- **Android Remote:** ✓ Web console, Cloud Shell from phone

### Dependencies
- Python 3.8+ (89.9% of codebase)
- kubectl CLI
- gcloud CLI (for GCP)
- Docker (for containerization)

---

## 🎯 RECOMMENDATION MATRIX

| Use Case | Best Choice | Why |
|----------|-------------|-----|
| **Production K8s Deployments** | wshobson/agents | Most comprehensive, enterprise-ready |
| **Troubleshooting & Incidents** | ahmedasmar/devops-claude-skills | Best diagnostics, playbooks |
| **Helm Charts** | wshobson/agents | Advanced chart development |
| **GitOps Implementation** | ahmedasmar/devops-claude-skills | ArgoCD + Flux expertise |
| **GCP/GKE Focus** | mrgoonie/claudekit-skills | GCP integration |
| **Security Policies** | wshobson/agents | Comprehensive security configs |
| **Multi-Cluster** | wshobson/agents | Best multi-cluster patterns |
| **Monitoring Setup** | ahmedasmar/devops-claude-skills | Prometheus, Grafana, tracing |
| **Learning K8s** | wshobson/agents | Best practices built-in |
| **Quick Deployments** | mrgoonie/claudekit-skills | Faster setup, cloud-native |

---

## 💡 QUICK START GUIDE

### For Production Deployments (wshobson):
```bash
# Install
/plugin install kubernetes-operations

# Use in Claude Code
"Create a production Deployment with:
- Nginx 1.21
- 3 replicas
- Rolling update strategy
- Liveness and readiness probes
- Resource limits: 200m CPU, 256Mi memory
- Service with LoadBalancer
- Ingress with TLS"

# Claude generates complete, production-ready manifests
```

### For Troubleshooting (ahmedasmar):
```bash
# Install
/plugin install k8s-troubleshooter@devops-skills

# Use in Claude Code
"My pod is stuck in CrashLoopBackOff. Help me diagnose."

# Claude provides systematic troubleshooting steps:
# 1. Check pod logs
# 2. Describe pod for events
# 3. Check resource constraints
# 4. Verify image availability
# 5. Check ConfigMaps/Secrets
# 6. Review security context
```

### For GKE Deployment (mrgoonie):
```bash
# Install
git clone https://github.com/mrgoonie/claudekit-skills.git
cp -r claudekit-skills/devops ~/.claude/skills/

# Use in Claude Code
"Deploy my Node.js app to GKE with:
- Autopilot cluster
- Cloud SQL database
- Cloud Storage bucket
- Workload Identity"

# Claude generates GKE-specific configs
```

---

## 📊 COMPARATIVE FEATURE MATRIX

| Feature | wshobson | ahmedasmar | mrgoonie |
|---------|----------|------------|----------|
| **Core Kubernetes** |
| Deployment Manifests | ✓✓✓ | ✓✓ | ✓✓ |
| StatefulSets | ✓✓✓ | ✓✓ | ✓ |
| DaemonSets | ✓✓✓ | ✓✓ | ✓ |
| Jobs/CronJobs | ✓✓✓ | ✓✓ | ✓ |
| Services | ✓✓✓ | ✓✓ | ✓✓ |
| Ingress | ✓✓✓ | ✓✓ | ✓✓ |
| ConfigMaps/Secrets | ✓✓✓ | ✓✓✓ | ✓✓ |
| **Advanced Features** |
| Helm Charts | ✓✓✓ | ✓✓ | ✓ |
| Kustomize | ✓✓ | ✓✓ | ✓ |
| Network Policies | ✓✓✓ | ✓✓ | ✓ |
| RBAC | ✓✓✓ | ✓✓ | ✓ |
| Pod Security | ✓✓✓ | ✓✓ | ✓ |
| HPA/VPA | ✓✓✓ | ✓✓✓ | ✓✓ |
| **GitOps** |
| ArgoCD | ✓✓✓ | ✓✓✓ | ✓ |
| Flux CD | ✓✓✓ | ✓✓✓ | ✓ |
| Multi-cluster | ✓✓✓ | ✓✓ | ✓ |
| **Operations** |
| Troubleshooting | ✓✓ | ✓✓✓ | ✓ |
| Monitoring Setup | ✓✓ | ✓✓✓ | ✓✓ |
| Incident Response | ✓✓ | ✓✓✓ | ✓ |
| Performance Tuning | ✓✓ | ✓✓✓ | ✓ |
| **Cloud Integration** |
| AWS EKS | ✓✓ | ✓✓✓ | ✓ |
| GCP GKE | ✓✓ | ✓✓ | ✓✓✓ |
| Azure AKS | ✓✓ | ✓✓ | ✓ |
| **Documentation** |
| Examples | ✓✓✓ | ✓✓✓ | ✓✓ |
| Best Practices | ✓✓✓ | ✓✓✓ | ✓✓ |
| Tutorials | ✓✓ | ✓✓ | ✓ |
| **Maintenance** |
| Active Development | ✓✓✓ | ✓✓✓ | ✓✓✓ |
| Community Support | ✓✓ | ✓✓ | ✓✓ |
| Issue Response | ✓✓ | ✓✓✓ | ✓✓ |

**Legend:** ✓✓✓ Excellent | ✓✓ Good | ✓ Basic | - Not Available

---

## 🚀 INSTALLATION RECOMMENDATION

**Best Approach: Install Top 2**

The best combination provides complete K8s coverage:

### Primary: wshobson/agents
For comprehensive K8s development and deployment

### Secondary: ahmedasmar/devops-claude-skills
For troubleshooting and GitOps

```bash
# One-liner installation
/plugin install kubernetes-operations && \
/plugin marketplace add https://github.com/ahmedasmar/devops-claude-skills && \
/plugin install k8s-troubleshooter@devops-skills && \
/plugin install gitops-workflows@devops-skills && \
echo "✓ Complete K8s skill suite installed!"
```

**Add mrgoonie if:** You primarily use GCP/GKE

---

## 🔧 CONFIGURATION EXAMPLES

### Production Deployment (wshobson)
```bash
# Ask Claude:
"Generate complete K8s manifests for production deployment:

Application: E-commerce API
- Language: Go
- Replicas: 5
- Resources: 500m CPU, 1Gi memory
- Database: PostgreSQL (external)
- Cache: Redis (StatefulSet)
- Queue: RabbitMQ (Helm chart)
- Ingress: nginx with TLS
- Monitoring: Prometheus metrics
- Security: NetworkPolicy, non-root user
- GitOps: ArgoCD application"

# Claude generates ~15 properly configured YAML files
```

### Troubleshooting (ahmedasmar)
```bash
# Ask Claude:
"Troubleshoot this issue:

Symptom: API pods keep restarting
Error: Connection timeout to database
Namespace: production
Cluster: AWS EKS"

# Claude provides systematic diagnostic approach:
# 1. Network policy check
# 2. Service discovery verification
# 3. DNS resolution test
# 4. Security group validation
# 5. Database connectivity test
# 6. Pod logs analysis
# Plus: kubectl commands to run for each step
```

### GKE Deployment (mrgoonie)
```bash
# Ask Claude:
"Deploy to GKE with GCP integrations:

App: Python Flask API
GKE: Autopilot cluster (us-central1)
Database: Cloud SQL PostgreSQL
Storage: Cloud Storage bucket
Secrets: Secret Manager
Identity: Workload Identity
Monitoring: Cloud Monitoring"

# Claude generates GKE-optimized configs with GCP resource bindings
```

---

## 📱 ANDROID ACCESS STRATEGY

While you cannot run K8s skills natively on Android, you can:

### ✓ What Works:
1. **SSH to Linux desktop**
   ```bash
   # From Android terminal (Termux)
   ssh user@linux-desktop
   kubectl get pods
   ```

2. **Cloud Shell from Android**
   - GCP Cloud Shell app
   - AWS CloudShell (web)
   - kubectl in browser

3. **K8s Dashboard (Web)**
   - Access via browser
   - View cluster status
   - Basic operations

4. **Lens IDE (Remote)**
   - SSH tunnel from Android
   - Web-based K8s management

5. **Git operations**
   - Edit manifests on Android
   - Commit and push
   - ArgoCD auto-syncs

### ✗ What Doesn't Work:
- Running Claude Code locally on Android
- Direct kubectl execution on Android
- Native skill execution
- Container runtime access

### Recommended Hybrid Workflow:
```
[Linux Desktop]               [Android Phone]
     ↓                             ↓
Generate manifests           Edit YAML files
Execute kubectl          →   Git commit & push
Monitor clusters         →   View dashboards
Troubleshoot issues      →   Alert notifications
     ↓                             ↓
     └─── ArgoCD GitOps ──────────┘
           (Auto-sync)
```

---

## 🐛 TROUBLESHOOTING SKILLS INSTALLATION

### Issue: Plugin not loading
```bash
# Check Claude Code plugin directory
ls -la ~/.claude/skills/

# Verify SKILL.md exists
cat ~/.claude/skills/kubernetes-operations/SKILL.md

# Check YAML frontmatter
head -10 ~/.claude/skills/kubernetes-operations/SKILL.md
```

### Issue: Skills not activating
```bash
# Check skill description in SKILL.md matches your request
# Skills activate based on description keywords

# Example: If asking "Create a K8s deployment"
# Make sure skill description includes "Kubernetes" or "deployment"
```

### Issue: Missing kubectl
```bash
# Install kubectl
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl

# Verify
kubectl version --client
```

---

## 📖 LEARNING RESOURCES

### Official Kubernetes Documentation
- https://kubernetes.io/docs/
- https://kubernetes.io/docs/concepts/
- https://kubernetes.io/docs/tutorials/

### Helm
- https://helm.sh/docs/
- https://artifacthub.io/

### GitOps
- https://argo-cd.readthedocs.io/
- https://fluxcd.io/docs/

### Best Practices
- https://kubernetes.io/docs/concepts/configuration/overview/
- https://cloud.google.com/kubernetes-engine/docs/best-practices

### Troubleshooting
- https://kubernetes.io/docs/tasks/debug/
- https://learnk8s.io/troubleshooting-deployments

---

## 🏆 FINAL RECOMMENDATIONS

### For Most Users:
**Install: wshobson/agents + ahmedasmar/devops-claude-skills**

This combination provides:
- Complete K8s manifest generation
- Production-ready configurations
- Troubleshooting capabilities
- GitOps implementation
- Monitoring setup
- Security policies

### For GCP Users:
**Add: mrgoonie/claudekit-skills**

Additional GKE-specific features and GCP integrations.

### Installation Priority:
1. **wshobson/agents** - Core K8s capabilities
2. **ahmedasmar/devops-claude-skills** - Operations & troubleshooting
3. **mrgoonie/claudekit-skills** - Optional, for GCP users

---

**Last Updated:** 2025-12-21
**Repositories Evaluated:** 3
**Category:** Kubernetes Orchestration & Cluster Management
**Skill Count:** 10+ K8s-focused skills across repositories
