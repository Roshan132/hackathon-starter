Kaibur Assessment

Table of Contents
	Overview
o	In this document, I have successfully implemented a Continuous Integration (CI) pipeline for given Node.js application. This pipeline includes thorough code quality checks and image scanning. Additionally, I have implemented Continuous Deployment (CD) using Helm charts. Furthermore, I have seamlessly configured an Azure Virtual Machine (VM) using Terraform and accomplished the installation of MongoDB utilizing Ansible.

	Prerequisites
o	Github account, Virtual machine, Any one cloud for Testing, Kubernetes, Helm, Terraform, Ansible, ArgoCd
	GitHub Repository Structure
o	Top of the repo inside .Github folder I have created action and workflow file for CI and CD workflow, I kept the helm charts inside Helm folder and Terraform files with the name of terraform and you can find the ansible also.
	GitHub Actions Workflow
o	Below is the Action Workflow structure:
o	 
o	I have implemented separate action files for all the steps of CI and calling that steps in workflow file named hackthon-CI 
	Helm Charts Deployment
o	I have designed the Helm charts to deploy it seamlessly in multiple environment just by updating the values.yaml 
o	The files you can find inside the helm folder in the repo
o	
	CD Workflow 
                      I have designed the CD workflow to Deploy the helm chart in AKS  with my own strategy 
 Written one shell script to check for the latest pushed image value in to the Azure container Registry and update the value in Values.yaml
So that it can deploy the charts using Helm upgrade –install command 
	Terrafrom to deploy Azure VM 
	             -   I have written a terraform script to deploy a Azure Virtual machine 


	Ansible SetUp to install MongoDB 
	          Designed Ansible playbook to install MongoDB 
	         
