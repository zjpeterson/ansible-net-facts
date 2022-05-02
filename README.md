# ansible-net-facts

This is a Network fact discovery demo I put together for Red Hat Automation Everywhere events, showcasing the following capabilities of Ansible:

* ServiceNow CMDB used as dynamic inventory
* Network Fact gathering
* ServiceNow CMDB data population

## Credentials

### Network

Provide a Machine credential (Tower/Controller) or set `ansible_user` / `ansible_password`.

### ServiceNow

You are expected to provide the ServiceNow host and login information via environment variables, such as `SN_USERNAME`. Refer to the `servicenow.itsm` collection documentation.

FYI, there is a playbook available at https://github.com/zjpeterson/ansible-tower-credential-types/blob/main/playbook_servicenow.yml that will create a ServiceNow credential type in Ansible Tower.
