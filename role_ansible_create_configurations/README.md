Role Name
=========

- role_ansible_create_configurations

      This role create configurations/components like credentials, hosts, inventories, templates, workflows, custom credentials etc in ansible tower

Role Variables
--------------

- category
- tower_gui_url
- tower_gui_username
- tower_gui_password
- payload
- method

Dependencies
------------

NA

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
         - role_ansible_pre_check
      vars:
        tower_gui_url: "http://10.0.0.1"
        tower_gui_username: "admin"
        tower_gui_password: "password"
        category: "projects"
        method: POST
        payload: { "name": "test_project", "description": "test project to configure tower", "organization": "default", "scm_url": "<taget url>", "scm_branch": "<target branch>", "scm_clean": true, "scm_delete_on_update": false, "credential": "<credential id", "scm_type": "git" }
Testing Platform
----------------

- Red Hat Enterprise Linux Server release 7.6 (Maipo)

Author Information
------------------

- Yasin Faizan S MD
