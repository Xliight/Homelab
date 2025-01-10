🏠 Homelab
This repo contains all of the configuration and documentation of my homelab.

The purpose of my homelab is to learn and to have fun. Being a Backend & Devops Engineer by trade, I work with Kubernetes every day, and my homelab is the place where I can try out and learn new things. On the other hand, by self-hosting some applications, it makes me feel responsible for the entire process of deploying and maintaining an application from A to Z. It forces me to think about backup strategies, security, scalability and the ease of deployment and maintenance.

Principles
I have a few principles that guide my choices for my homelab.

Storage is provisioned in local database and i will do backups in AWS Cloud
I aim to adopt best practices in deployment and security
Everything is deployed through GitOps
When selecting self hosted options, I always opt for the ones that allow me to run a separate Postgres database that I can manage myself
Cluster Provisioning
I use KubeAdm my machines. I love Talos because it is so lightweight and minimal, and it provides production grade security right out of the box. It also forces me to use all my servers as Kubernetes nodes only, so I need to figure out ways to run all my desired workloads and services on Kubernetes.

I use Proxmox as a hypervisor to provision VMs

Hardware
I'm running a production cluster. 😏

I use a old laptops and sometimes a few virtual machines..


controlplane-1 4C/4GB
worker-1/2 4C/4GB running Ubuntu Desktop. This is my personal machine and I sometimes add a few VMs  when I need them.

Secrets
Secrets are synced to HashiCorp  Vault
SAS tokens for Storage Account Access# Homelab
