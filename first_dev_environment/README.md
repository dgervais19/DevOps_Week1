# Intro to DevOps

* Agile Practices:
	- working software, over documentation
	- customer collaboration
	- individual interactions over the process
	- responding

* Internal culture:
	- CI/CD Pipelines
	- Continous Testing
	- Standardized Enviroments
	- Whilest keeping cost low, and  handling peaks and growth

* 4 Pillars of DevOps:
	- Ease of use
	- Flexibility
	- Robustness
	- Cost

A succesful DevOps implementation turns challenges into benefits

* Stages in DevOps Lifecylce:
	- Continuous Integration
	- Continuous Deliver
	- Continuous Deployment
	- Continuous Testing
	- Continuous Monitoring

### DevOps Implementation
* Cloud Platform:
	- AWS
	- GCP
	- Azure

* Infrastructure Architecture:
	- Virtualization
	- Containerization (Docker)

* DevOps Implementations:
	- Infrastructure as Code (IAC)
	- Infrastructure as a service (IaaS)
	- Infrastructure as a platform (IaaP)
	- Infrastructure as a product

## Environments
* Where code runs
* Github, is not an enviroment. But pycharm and computers are environments
* Pycharm:
	- Creates individual virtual environments -> venv folder
	- Robustness

### 3 Main Environments
* Dev Environment
* Testing Environment
* Deployment/Live Environment

## First Virtual Box, Vagrant Dev Environment

This repo is our first virtual environment to create a dev environment.

### **Virtual Box**
**What is it?**
* It allows multiple OS's to be running at the same time
* It facillitates testing and disater recovery

**Terminology**
* `Host OS` - The computer that the VM runs on
* `Guest OS` - The virtual OS that is running on the VM
* `Virtual Machine` - The environment that allows the guest OS to run.

### **Vangrant**

**What is it?**
* It is an open source tool which is used to build and manage virtual environments
* Vagrant helps to lower development environment time.
* Vagrant will create the VM ensuring that it is set up to industry-standard through using provisioning tools such as shell scripts.

**Vangrant boxes** 
* pre leaded vagrant files that create virtual machines. Usually just an OS.
* Common OS's include Ubuntu and Windows
	- Ubuntu with GUI (Graphical User Interface) is an OS like Windows or MacOS where the UI has graphics making it easier to use.
	- Ubuntu Headless just uses the terminal

**Ubuntu:**
- is an open source OS
- With GUI it looks like a desktop and works like one.
- Headless is basically a terminal, no GUI. (This is the one we will use)
- faster
- more secure
 - lighter

**Main commands**
- `vagrant init` - Creates a `vagrantfile` in the directory that you're in
- `vagrant init <box name>` - search for boxes in https://app.vagrantup.com/ to create a specific box with
- `vagrant up` - creates a virtual machine using the info from the `vagrantfile`
- `vagrant destroy` - destroys the entire VM
- `vagrant ssh` - Once you have started up your VM, this logs in to the Guest OS allowing you to use its terminal through your normal computer.
- `vagrant reload` - basically `vagrant halt` and then `vagrant up`... this is used once you make changes within your VM and you want to see them.

## Linux
**NGINX**
* Once loaded into an Ubuntu VM, one can install 'nginx' with the command `sudo apt install nginx`
* Open-source software for web servering and reverse proxying
* It's faster than most web servers like Apache

**Linux Terminal Commands**
* `sudo` - allows you to use commands as admin
* `sudo apt update` - see apps
* `sudo apt instal <package name>` - install a specific package
