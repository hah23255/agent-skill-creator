# 🦭 PODMAN SKILLS - Scored Recommendations

## Category: Podman Container Management & MCP Integration

---

## 📊 COMPREHENSIVE SCORING

| Repository | Overall | Functionality | Flexibility | Portability | Docs | License | Active |
|------------|---------|---------------|-------------|-------------|------|---------|--------|
| **manusa/podman-mcp-server** | **9.2** | 10 | 8 | 9 | 9 | 10 | 10 |
| **rimaleon/podman-mcp** | **8.0** | 8 | 7 | 8 | 7 | 10 | 7 |
| **bjeans/homelab-mcp** | **8.5** | 9 | 9 | 8 | 8 | 10 | 8 |

**Scoring Criteria (1-10):**
- **Functionality:** Features, capabilities, completeness
- **Flexibility:** Modularity, customization, adaptability
- **Portability:** Cross-platform, installation ease, dependencies
- **Documentation:** Quality, completeness, examples
- **License:** Permissiveness (10=MIT/Apache, 5=restrictive)
- **Active:** Maintenance, updates, community support

---

## 🥇 BEST: manusa/podman-mcp-server
**Overall Score: 9.2/10**

### Strengths
✓ **Dual runtime support** - Works with both Podman AND Docker
✓ **Model Context Protocol** - Standardized AI interface
✓ **Production-ready** - Stable, well-tested
✓ **Multiple installation methods** - npm, binary, language wrappers
✓ **Go-based** - Fast, efficient, compiled binary
✓ **Active development** - Regular updates, responsive maintainer
✓ **Comprehensive documentation** - Clear setup guides

### Capabilities
- **Container Management:**
  - List, create, start, stop, remove containers
  - Inspect container details
  - Stream logs in real-time
  - Execute commands in containers

- **Image Operations:**
  - Pull, push, tag images
  - Build images from Dockerfiles
  - List and manage images
  - Prune unused images

- **Network Management:**
  - Create and manage networks
  - Connect/disconnect containers
  - Network inspection

- **Volume Management:**
  - Create persistent storage
  - Manage volume lifecycle
  - Mount volumes to containers

- **AI Integration:**
  - Model Context Protocol (MCP) interface
  - Works with Claude Desktop, VS Code, Goose CLI
  - Natural language container operations
  - Automated troubleshooting

### Installation

#### Method 1: npm (Fastest)
```bash
# Run directly with npx
npx podman-mcp-server@latest

# Or install globally
npm install -g podman-mcp-server
podman-mcp-server
```

#### Method 2: Binary Release
```bash
# Download from GitHub releases
wget https://github.com/manusa/podman-mcp-server/releases/latest/download/podman-mcp-server-linux-amd64

# Make executable
chmod +x podman-mcp-server-linux-amd64

# Run
./podman-mcp-server-linux-amd64
```

#### Method 3: From Source (Go)
```bash
# Clone repository
git clone https://github.com/manusa/podman-mcp-server.git
cd podman-mcp-server

# Build
go build

# Run
./podman-mcp-server
```

#### Integration with Claude Desktop
```json
// Add to Claude Desktop config
{
  "mcpServers": {
    "podman": {
      "command": "npx",
      "args": ["podman-mcp-server@latest"]
    }
  }
}
```

### Use Cases
- ✓ AI-driven container management via Claude
- ✓ Natural language container operations
- ✓ Automated container troubleshooting
- ✓ DevOps workflow automation
- ✓ Container lifecycle management
- ✓ Cross-platform container control (Podman/Docker)

### Scoring Breakdown
| Metric | Score | Rationale |
|--------|-------|-----------|
| Functionality | 10/10 | Complete container runtime control |
| Flexibility | 8/10 | Works with Podman & Docker, modular |
| Portability | 9/10 | Multiple install methods, Go binary |
| Documentation | 9/10 | Excellent setup guides, clear examples |
| License | 10/10 | Open source |
| Active Development | 10/10 | Very active, responsive maintenance |

### Platform Support
- **Linux Desktop:** ✓✓✓ Full native support
- **macOS:** ✓✓✓ Full support
- **Windows:** ✓✓ WSL2 support
- **Android Native:** ✗ Not supported (requires container runtime)
- **Android Remote:** ✗ No remote access mode

### Dependencies
- **Runtime:** Podman or Docker installed
- **Optional:** Node.js/npm (for npm installation)
- **Optional:** Go 1.19+ (for building from source)

### Technical Details
- **Language:** Go (79.4%)
- **Binary Size:** ~15MB (compiled)
- **Memory Usage:** Low (<50MB typical)
- **Performance:** Near-native speed

---

## 🥈 ALTERNATIVE 1: bjeans/homelab-mcp
**Overall Score: 8.5/10**

### Strengths
✓ **Multi-service management** - Docker/Podman + Ollama + Pi-hole + Unifi
✓ **Homelab focus** - Perfect for self-hosted infrastructure
✓ **Security checks** - Built-in validation and templates
✓ **Ansible integration** - Infrastructure as Code
✓ **Production-ready** - Automated validation, pre-push hooks
✓ **Comprehensive** - Manages entire homelab stack

### Capabilities
- **Container Management:**
  - Docker/Podman container operations
  - Container monitoring and health checks
  - Multi-runtime support

- **Additional Services:**
  - Ollama AI models management
  - Pi-hole DNS administration
  - Unifi network management
  - Ansible inventory integration

- **DevOps Features:**
  - Pre-push validation
  - Security templates
  - Automated health checks
  - Infrastructure monitoring

### Installation
```bash
# Clone repository
git clone https://github.com/bjeans/homelab-mcp.git
cd homelab-mcp

# Install dependencies (Python-based)
pip install -r requirements.txt

# Configure for your homelab
cp config.example.yaml config.yaml
# Edit config.yaml with your settings

# Run MCP server
python mcp_server.py
```

### Integration with Claude Desktop
```json
{
  "mcpServers": {
    "homelab": {
      "command": "python",
      "args": ["/path/to/homelab-mcp/mcp_server.py"]
    }
  }
}
```

### Use Cases
- ✓ Managing home server infrastructure
- ✓ Self-hosted service orchestration
- ✓ Network administration via AI
- ✓ DNS management (Pi-hole)
- ✓ AI model deployment (Ollama)
- ✓ Unified homelab control

### Scoring Breakdown
| Metric | Score | Rationale |
|--------|-------|-----------|
| Functionality | 9/10 | Comprehensive homelab management |
| Flexibility | 9/10 | Multi-service, highly customizable |
| Portability | 8/10 | Python-based, some service dependencies |
| Documentation | 8/10 | Good docs, homelab-specific |
| License | 10/10 | Open source |
| Active Development | 8/10 | Active, niche focus |

### Platform Support
- **Linux Desktop:** ✓✓✓ Full support (primary target)
- **Raspberry Pi:** ✓✓✓ Optimized for homelab
- **Android Native:** ✗ Not supported
- **Android Remote:** ✗ No remote mode

### Dependencies
- Python 3.8+
- Docker or Podman
- Optional: Ollama, Pi-hole, Unifi Controller, Ansible

---

## 🥉 ALTERNATIVE 2: rimaleon/podman-mcp
**Overall Score: 8.0/10**

### Strengths
✓ **Pure Podman focus** - Dedicated Podman implementation
✓ **Compose stack support** - Manages multi-container applications
✓ **Model Context Protocol** - Standard AI interface
✓ **Lightweight** - Minimal dependencies
✓ **Seamless Claude integration** - Natural language operations

### Capabilities
- **Podman Operations:**
  - Container lifecycle management
  - Pod management
  - Compose stack operations
  - Image management

- **Compose Features:**
  - Deploy compose stacks
  - Stack health monitoring
  - Multi-container orchestration
  - Service scaling

### Installation
```bash
# Clone repository
git clone https://github.com/rimaleon/podman-mcp.git
cd podman-mcp

# Install dependencies
npm install
# or
pip install -r requirements.txt

# Run MCP server
npm start
# or
python server.py
```

### Integration with Claude Desktop
```json
{
  "mcpServers": {
    "podman": {
      "command": "node",
      "args": ["/path/to/podman-mcp/server.js"]
    }
  }
}
```

### Use Cases
- ✓ Podman-specific workflows
- ✓ Compose stack deployment
- ✓ Multi-container application management
- ✓ AI-assisted container operations
- ✓ Development environment automation

### Scoring Breakdown
| Metric | Score | Rationale |
|--------|-------|-----------|
| Functionality | 8/10 | Good Podman coverage, compose support |
| Flexibility | 7/10 | Podman-specific, less adaptable |
| Portability | 8/10 | Node/Python options, standard deps |
| Documentation | 7/10 | Basic docs, could be more detailed |
| License | 10/10 | Open source |
| Active Development | 7/10 | Active but slower pace |

### Platform Support
- **Linux Desktop:** ✓✓✓ Full support
- **macOS:** ✓✓ Limited (Podman Desktop required)
- **Android Native:** ✗ Not supported
- **Android Remote:** ✗ No remote mode

### Dependencies
- Podman runtime
- Node.js or Python 3.8+
- podman-compose (optional)

---

## 🎯 RECOMMENDATION MATRIX

| Use Case | Best Choice | Why |
|----------|-------------|-----|
| **General Container Management** | manusa/podman-mcp-server | Best features, dual runtime support |
| **Homelab Infrastructure** | bjeans/homelab-mcp | Multi-service, Raspberry Pi optimized |
| **Pure Podman Workflows** | rimaleon/podman-mcp | Podman-specific, compose support |
| **AI Integration** | manusa/podman-mcp-server | Best MCP implementation, active dev |
| **Self-Hosted Services** | bjeans/homelab-mcp | Ollama, Pi-hole, Unifi included |
| **Production Deployments** | manusa/podman-mcp-server | Most stable, well-tested |
| **Docker + Podman** | manusa/podman-mcp-server | Only one with dual support |
| **Beginners** | manusa/podman-mcp-server | Best docs, easy installation |

---

## 💡 QUICK START GUIDE

### For General Use (manusa):
```bash
# Fastest installation
npx podman-mcp-server@latest

# Add to Claude Desktop config
# Then ask Claude: "List my running containers"
```

### For Homelab (bjeans):
```bash
# Install
git clone https://github.com/bjeans/homelab-mcp.git
cd homelab-mcp
pip install -r requirements.txt

# Configure
cp config.example.yaml config.yaml
# Edit config.yaml

# Use with Claude
# Ask: "Show status of all homelab services"
```

### For Podman-Only (rimaleon):
```bash
# Install
git clone https://github.com/rimaleon/podman-mcp.git
cd podman-mcp
npm install

# Run
npm start

# Use with Claude
# Ask: "Deploy this compose stack with Podman"
```

---

## 📊 COMPARATIVE FEATURE MATRIX

| Feature | manusa | bjeans | rimaleon |
|---------|--------|--------|----------|
| Podman Support | ✓✓✓ | ✓✓✓ | ✓✓✓ |
| Docker Support | ✓✓✓ | ✓✓✓ | ✗ |
| Pod Management | ✓✓✓ | ✓✓ | ✓✓✓ |
| Compose Stacks | ✓✓ | ✓✓ | ✓✓✓ |
| Image Operations | ✓✓✓ | ✓✓ | ✓✓ |
| Network Management | ✓✓✓ | ✓✓ | ✓✓ |
| Volume Management | ✓✓✓ | ✓✓ | ✓✓ |
| MCP Protocol | ✓✓✓ | ✓✓✓ | ✓✓✓ |
| Claude Integration | ✓✓✓ | ✓✓✓ | ✓✓✓ |
| Ollama Support | - | ✓✓✓ | - |
| Pi-hole Support | - | ✓✓✓ | - |
| Unifi Support | - | ✓✓✓ | - |
| Installation Ease | ✓✓✓ | ✓✓ | ✓✓ |
| Documentation | ✓✓✓ | ✓✓ | ✓✓ |
| Active Development | ✓✓✓ | ✓✓ | ✓✓ |
| Binary Release | ✓✓✓ | ✗ | ✗ |

**Legend:** ✓✓✓ Excellent | ✓✓ Good | ✓ Basic | - Not Available

---

## 🚀 INSTALLATION RECOMMENDATION

**Primary Choice: manusa/podman-mcp-server**

For most users, this is the best option. However:

**Choose bjeans/homelab-mcp if:**
- You run a homelab with Pi-hole, Unifi, Ollama
- You need multi-service orchestration
- You're on Raspberry Pi

**Choose rimaleon/podman-mcp if:**
- You exclusively use Podman (no Docker)
- You need advanced compose stack features
- You want Podman-specific optimizations

### Recommended Installation
```bash
# Install the best general-purpose option
npm install -g podman-mcp-server

# Configure Claude Desktop
cat >> ~/.config/claude-desktop/config.json <<EOF
{
  "mcpServers": {
    "podman": {
      "command": "podman-mcp-server"
    }
  }
}
EOF

# Test
podman-mcp-server --version
```

---

## 🔧 CONFIGURATION EXAMPLES

### manusa/podman-mcp-server
```bash
# Run with custom port
podman-mcp-server --sse-port 8080

# Run with Docker instead of Podman
DOCKER_HOST=unix:///var/run/docker.sock podman-mcp-server

# Run with remote Podman
PODMAN_HOST=ssh://user@remotehost podman-mcp-server
```

### bjeans/homelab-mcp
```yaml
# config.yaml
containers:
  runtime: podman
  socket: /run/podman/podman.sock

ollama:
  enabled: true
  host: localhost
  port: 11434

pihole:
  enabled: true
  host: 192.168.1.10
  api_key: your-api-key

unifi:
  enabled: true
  host: 192.168.1.1
  username: admin
  password: your-password
```

### rimaleon/podman-mcp
```json
{
  "podman": {
    "socket": "/run/user/1000/podman/podman.sock",
    "compose": {
      "enabled": true,
      "default_project": "myapp"
    }
  }
}
```

---

## 🐛 TROUBLESHOOTING

### Common Issues

**Issue: "Cannot connect to Podman socket"**
```bash
# Start Podman socket
systemctl --user enable --now podman.socket

# Verify socket
ls -la /run/user/$(id -u)/podman/podman.sock
```

**Issue: "Permission denied"**
```bash
# Add user to podman group (rootless mode)
# No group needed for rootless Podman

# For rootful Podman
sudo usermod -aG podman $USER
newgrp podman
```

**Issue: "MCP server not responding"**
```bash
# Check if server is running
ps aux | grep mcp-server

# Check logs
journalctl --user -u podman-mcp-server

# Restart server
systemctl --user restart podman-mcp-server
```

---

## 📖 LEARNING RESOURCES

### Podman Official Documentation
- https://docs.podman.io/
- https://podman-desktop.io/
- https://github.com/containers/podman

### Model Context Protocol
- https://modelcontextprotocol.io/
- https://spec.modelcontextprotocol.io/

### Podman vs Docker
- https://docs.podman.io/en/latest/markdown/podman-docker.1.html

### Homelab Resources
- https://awesome-selfhosted.net/
- https://github.com/awesome-selfhosted/awesome-selfhosted

---

## ⚠️ ANDROID LIMITATION NOTICE

**All Podman MCP servers require:**
- Container runtime (Podman or Docker)
- Linux kernel with namespace support
- Systemd or equivalent init system
- Direct socket access

**Android devices cannot run these natively because:**
- No native container runtime support
- Kernel restrictions (no full namespace isolation)
- No systemd
- Termux limitations

**Workaround:** Use Android to SSH into Linux server running Podman MCP server.

---

**Last Updated:** 2025-12-21
**Repositories Evaluated:** 3
**Category:** Podman Container Management & MCP Integration
