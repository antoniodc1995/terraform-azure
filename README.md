# terraform-azure
Dev Environment on Azure with Terraform

## Introduction
This Terraform configuration file is used to deploy a Dev Environment on Microsoft Azure. The setup includes a resource group, a virtual network, a subnet, a network security group, a public IP, a network interface, and a Linux virtual machine. Additionally, it outputs the public IP address of the deployed virtual machine.

## Resources Created
1. Resource Group: mtc-resources in West Europe.
2. Virtual Network: mtc-network with address space 10.123.0.0/16.
3. Subnet: mtc-subnet with address prefix 10.123.0.0/24.
4. Network Security Group: mtg-sg with a rule allowing all inbound traffic.
5. Public IP: mtc-ip with dynamic allocation.
6. Network Interface: mtc-nic connected to the public IP and subnet.
7. Linux Virtual Machine: mtc-vm using an Ubuntu 18.04-LTS image, with a dynamic private IP and public IP.