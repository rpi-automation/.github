_I'm moving this organization to codeberg repo https://codeberg.org/publowski/rpi-automation _

# Raspberry Pi Automation

This project aims to provide a comprehensive automation infrastructure for Raspberry Pi devices, leveraging Ansible and workflow automation tools to simplify management and boost productivity.

## Repositories Overview

### infra-ansible

This repository contains Ansible playbooks and roles designed to automate the infrastructure setup and configuration of Raspberry Pi devices. 

### services-n8n

This repository hosts the configuration and workflows for deploying n8n, a powerful open-source workflow automation tool.

### Archive

Repository for all no longer used services, components. Maybe they'll be needed someday...

## Project Goals

* Simplify Raspberry Pi infrastructure provisioning through Ansible automation.
* Enable local and reliable workflow automation using n8n.
* Reduce manual configuration and increase operational efficiency.

### Feel free to explore the repositories, contribute, and share your feedback!

## Organisation changelog
* 17.12.2025 - infra-ansible - Added DNS (dnsmasq container for managing traefik domains without need to use hosts file), Simplified CICD
* 14.12.2025 - infra-ansible - Added (/returned to) traefik for all devices (was experimenting on custom url for each service but domains were better to maintain)
* 08.12.2025 - archive - Created Repository for no longer used services
* 06.12.2025 - infra-ansible - Changed 3d printer software from klipper,moonraker,fluidd combo to octoprint
* 30.11.2025 - infra-ansible - Added Zigbee bridge to Home Assistant
* 25.11.2025 - infra-ansible - Added notes services - Joplin server (for notes synchronisation), exclaidraw (hand writing, painting)
* 20.11.2025 - infra-ansible - Added HACS extention for Home Assistant container
* 17.11.2025 - infra-ansible - Added cypress container for future automated tests
* 12.11.2025 - infra-ansible - Added alerting services for future use (prometheus, alertmanager, cadvisor)
* 08.11.2025 - infra-ansible - Migrated Home Assitant from VM to contenerised version 
* 03.11.2025 - n8n-workflows - added repository which stores n8n workflows
* 03.11.2025 - rpi-automation - moved repository to it's own github organisation for better maintanance of whole project, created prpject to better track of issues
* 03.11.2025 - infra-ansible - Added n8n container and setup
* 30.10.2025 - infra-ansible - Modified CI slightly
* 29.10.2025 - infra-ansible - Added VPN container (wireguard)
* 27.10.2025 - infra-ansible - Added firewall (ufw)
* 23.10.2025 - infra-ansible - Added playbook which automatically completes onboarding setup for Home assistant
* 22.10.2025 - infra-ansible - Added Samba container
* 18.10.2025 - infra-ansible - Added Nginx container setup, and removed traefik form klipper
* 17.10.2025 - infra-ansible - Created playbook for Home Assistant VM, Created playybooks for remote managing my 3d printer (klipper, moonraker, fluidd)
* 16.10.2025 - infra-ansible - Added Cockpit UI for easier RaswpberryPi system management and added 3rd party extension for docker containers management, created issues for this repository
* 13.10.2025 - infra-ansible - Created fiirst ansible roles for docker containers and quemu VMs with simple Github Actions CI
* 05.10.2025 - infra-ansible - Created infra-ansible repository
