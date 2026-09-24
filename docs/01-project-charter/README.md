# OputGuard Enterprise Network Automation Platform

## 1. Project Overview

The OputGuard Enterprise Network Automation Platform is a production-inspired
multi-vendor enterprise infrastructure environment designed to develop,
validate and demonstrate modern network engineering, infrastructure automation,
cloud integration, DevOps and platform engineering practices.

The environment is operated as an engineering simulation rather than represented
as a real large-scale production enterprise. It is designed to reproduce
realistic enterprise requirements, change processes, incidents, migrations,
automation workflows and operational challenges.

The platform will also provide a controlled engineering environment for
OputGuard Technologies Ltd to develop and validate infrastructure automation
capabilities and future technology services.

---

## 2. Business Context

Modern enterprise networks increasingly require engineers to work beyond
traditional device-by-device configuration.

Network infrastructure is progressively managed through:

- Infrastructure as Code
- source-of-truth platforms
- APIs
- configuration templates
- automated validation
- CI/CD pipelines
- observability
- IT service management processes
- workflow automation
- AI-assisted operations

The project will establish an environment in which these technologies and
operational practices can be integrated and exercised through realistic
engineering scenarios.

---

## 3. Project Objectives

The project will:

1. Build a realistic multi-site enterprise network environment.

2. Implement multi-vendor routing, switching, firewall and SD-WAN
   technologies.

3. Establish repeatable network automation using Python, Ansible,
   APIs and configuration templates.

4. Apply Infrastructure as Code where appropriate.

5. Implement automated pre-change and post-change validation using
   pyATS/Genie and related tooling.

6. Introduce a source-of-truth approach for infrastructure data.

7. Develop CI/CD workflows for controlled network changes.

8. Implement monitoring, logging and operational observability.

9. Simulate enterprise incidents, migrations, failures and recovery
   procedures.

10. Introduce workflow orchestration and AI-assisted operational
    capabilities where they provide a justified engineering benefit.

11. Produce professional engineering documentation including HLDs,
    LLDs, implementation plans, test plans, rollback plans, change
    records, runbooks and incident reports.

---

## 4. Technology Domains

The programme may incorporate the following technologies as requirements
develop:

### Network and Security

- Cisco routing and switching
- Fortinet FortiGate
- Cisco Firepower
- OSPF
- BGP
- VLANs and inter-VLAN routing
- VPN
- SD-WAN
- network segmentation

### Network Automation

- Python
- Ansible
- Netmiko
- NAPALM
- Jinja2
- REST APIs
- pyATS
- Genie

### Infrastructure as Code

- Terraform
- Git-based infrastructure workflows

### Source of Truth

- NetBox

### CI/CD

- GitHub
- GitHub Actions
- Jenkins where justified

### Infrastructure Platforms

- VMware Workstation
- EVE-NG
- Linux
- Windows Server

### Cloud and Hybrid Infrastructure

- AWS
- Azure where justified
- hybrid connectivity
- cloud networking
- infrastructure automation

### Observability

- infrastructure monitoring
- metrics
- logging
- alerting

### Workflow and AI Automation

- n8n
- API-driven workflow orchestration
- AI-assisted analysis
- controlled AI-agent workflows

---

## 5. Environment Classification

The wider OputGuard technology environment will distinguish between:

### Production

Real services relied upon by OputGuard Technologies Ltd or its customers.
Production systems must not be intentionally disrupted for training purposes.

### Pre-Production

Systems used to validate releases, infrastructure changes and migrations
before production implementation.

### Engineering Simulation

A deliberately breakable environment used for infrastructure engineering,
automation development, incident simulation, troubleshooting and technical
experimentation.

The EVE-NG enterprise environment created by this project primarily belongs
to the Engineering Simulation classification.

---

## 6. Engineering Principles

The programme will follow the following principles:

- Infrastructure changes must originate from a defined requirement.
- Configuration should be repeatable wherever practical.
- Infrastructure state should be documented and version controlled.
- Automation must include validation rather than deployment alone.
- Changes should have defined success and rollback criteria.
- Credentials and secrets must not be committed to source control.
- Production services must remain isolated from destructive simulation.
- Monitoring and evidence should guide troubleshooting.
- Automation should not remove appropriate human approval and governance.
- New technologies should be introduced because they solve an engineering
  requirement, not simply to increase the number of tools in the project.

---

## 7. Initial Platform Architecture

The initial engineering platform consists of:

### EVE-NG

Provides network and security device emulation for enterprise network
topologies.

Initial available device families include:

- Cisco network devices
- FortiGate
- Cisco Firepower
- Linux systems
- Windows systems

### OGT-AUTO-01

Dedicated Ubuntu-based network automation control node.

Initial responsibilities include:

- Git operations
- Python automation
- Ansible
- pyATS / Genie
- Netmiko
- NAPALM
- API interaction
- Terraform
- network validation

### GitHub

Provides remote source control and will progressively support:

- branch-based development
- peer-review style workflows
- pull requests
- CI/CD
- engineering documentation
- version history

---

## 8. Delivery Approach

The platform will be developed incrementally.

Each significant infrastructure capability should progress through:

Requirement
→ Design
→ Implementation Plan
→ Automated/Manual Validation
→ Change
→ Post-Change Validation
→ Documentation
→ Review

Where appropriate, failures will be intentionally introduced into the
Engineering Simulation environment to develop troubleshooting and incident
management capability.

---

## 9. Target Engineering Capability

The programme is intended to develop the ability to design, implement,
automate, validate and troubleshoot enterprise network changes using modern
engineering practices.

Target capabilities include:

- infrastructure automation
- network configuration management
- Infrastructure as Code
- source-of-truth integration
- automated network validation
- CI/CD-driven change
- API integration
- implementation and migration
- troubleshooting across network and automation workflows
- operational governance
- continuous improvement

---

## 10. Success Criteria

The programme will be considered technically successful when the environment
can demonstrate an end-to-end controlled infrastructure change such as:

Requirement
→ source-of-truth update
→ Git change
→ automated validation
→ approval workflow
→ automated deployment
→ post-change validation
→ monitoring
→ documented outcome

The engineer should also be capable of diagnosing and recovering from
deliberately introduced failures across this workflow.

---

## 11. Current Status

Platform foundation established:

- EVE-NG 7 Community Edition operational
- network/security images available
- FortiGate successfully booted
- dedicated Ubuntu automation control node operational
- automation node has Internet and EVE-NG management connectivity
- Git repository migrated to the automation node
- Python virtual environment established
- Ansible operational
- pyATS/Genie operational
- GitHub SSH authentication operational

The next programme stage is formal enterprise architecture and network design.