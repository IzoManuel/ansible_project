# DG Ansible Project

## Description

This project aims to deploy a highly available and redundant infrastructure for hosting a personal resume website using Ansible. The infrastructure will be configured with multiple NGINX servers in an active-passive setup and duplicate web servers for high availability. The goal is to ensure that the website remains accessible and operational, even in the event of server failure.

## Installation

1. Clone the repository:

   ```bash
    git clone <repository-url>
    cd my_ansible_project

2. Set up a virtual environment (optional but recommended):

    ```bash
    virtualenv venv
    source venv/bin/activate

3. Install Ansible and pre-commit:

    ```bash
    pip install ansible pre-commit
    pre-commit install

4. Set up pre-commit hooks:
    ```bash
    pre-commit install

## Usage

1. Configure your inventory file (inventory/production/hosts) with the IP addresses or hostnames of your servers.

2. Modify the Ansible playbooks (site.yml, webservers.yml, nginx.yml) and roles (roles/) as needed to fit your project requirements.

3. Run Ansible playbooks to deploy your infrastructure:

    ```
    ansible-playbook -i inventory/production/hosts site.yml

## Pre-commit Hooks

This project uses pre-commit to enforce code quality and consistency. Before committing changes, pre-commit hooks will automatically run to check for issues such as linting errors and formatting violations.

To manually run pre-commit hooks:

    ```
    pre-commit run --all-files

## License

This project is licensed under the MIT License.

Feel free to customize and expand upon this template to better fit your project's specific needs and requirements.