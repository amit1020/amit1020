<h1 align="center">Amit Levi</h1>

<p align="center">
  <b>Computer Science student at Tel Aviv University</b><br>
  Infrastructure · Kubernetes · Platform Security
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/amit-levi-a61744215/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:amitlevi.tech@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
  <img src="https://img.shields.io/badge/AWS_Certified-SAA-FF9900?style=for-the-badge&logo=amazonwebservices&logoColor=white" />
</p>

<br>

I build infrastructure that is fully described in code. A system you cannot
rebuild from a repository is a system you do not fully understand — that idea
shapes most of what I work on.

I am finishing a B.Sc. in Computer Science at Tel Aviv University, and in
parallel I run a production-style Kubernetes platform at home: five nodes,
isolated network, every piece of state reconciled from Git. Most of what I know
about operating systems, networking and failure modes I learned by building that
and then fixing it when it broke.

Looking for a **DevOps / Platform Engineering** role — open to positions in
Israel and to relocation.

<br>

---

## Featured project

### [homelab](https://github.com/amit1020/homelab) — Kubernetes on Talos Linux

A five-node cluster running on Proxmox behind an isolated VLAN, reachable only
over WireGuard.

Machine configuration, network layout, workloads and SOPS-encrypted secrets all
live in the repository. Flux runs inside the cluster and reconciles it from Git,
so manual changes are reverted rather than accumulating as configuration drift.
Cilium provides the eBPF dataplane, NetworkPolicy and L2 load balancing —
replacing kube-proxy and MetalLB with a single component.

The repository also documents the design decisions and the incidents hit while
building it. The diagnostic reasoning turned out to be more reusable than the
fixes themselves.

<table>
<tr>
<td><b>OS</b></td><td>Talos Linux — immutable, API-driven, no SSH</td>
</tr>
<tr>
<td><b>Networking</b></td><td>Cilium (eBPF), MikroTik RouterOS, VLAN segmentation, WireGuard</td>
</tr>
<tr>
<td><b>GitOps</b></td><td>Flux — pull-based, no inbound access to the cluster</td>
</tr>
<tr>
<td><b>Secrets</b></td><td>SOPS + age, encrypted at rest in Git</td>
</tr>
</table>

<br>

---

## Technical focus

**Infrastructure as code** &nbsp;·&nbsp; Talos Linux, Proxmox, Terraform,
MikroTik RouterOS. Declarative configuration over imperative scripts — if it
needed a manual step, it is not finished.

**Kubernetes and networking** &nbsp;·&nbsp; Cilium with eBPF, NetworkPolicy,
GitOps with Flux, Helm and Kustomize. Service meshes, ingress, and the failure
modes that show up when a control plane loses quorum.

**Cloud** &nbsp;·&nbsp; AWS — Lambda, S3, API Gateway, DynamoDB, SAM,
CloudFormation. Serverless architectures and where they stop being the right
answer.

**Platform security** &nbsp;·&nbsp; Secret management with SOPS, least-privilege
credentials for automation, network segmentation as a design constraint rather
than an afterthought.

**Languages** &nbsp;·&nbsp; Python, C++, Java, Bash

<br>

---

## Education & certifications

**B.Sc. Computer Science** — Tel Aviv University *(in progress)*

| Certification | Issuer | Year |
| :--- | :--- | :--- |
| AWS Certified Solutions Architect – Associate | Amazon Web Services | 2025 |
| DevOps Professional Training | Sela College | 2024 – 2025 |
| Linux Essentials | ITSafe | 2024 |
| Python Development | ITSafe | 2021 |

<br>

---

## Background

IDF veteran — communications systems operator, and later company sergeant major.
The habits that came out of that service are the ones I still work by: document
what you change, assume the network is hostile, and never trust a configuration
you have not verified yourself.

<br>

---

<p align="center">
  <b>Hebrew</b> native &nbsp;·&nbsp; <b>English</b> professional<br>
  Based in Israel · open to relocation
</p>

<details>
<summary align="center">GitHub statistics</summary>
<br>
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=amit1020&show_icons=true&hide_border=true&theme=dark&count_private=true" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=amit1020&layout=compact&hide_border=true&theme=dark" />
</p>
</details>
