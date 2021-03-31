Role Name
=========

- role_ansible_clone_git_repo

      This role clones the git repository to the localhost

Role Variables
--------------

- git_repo_url
- branch
- clone_dest_path
- bb_username
- bb_password

Dependencies
------------

- NA

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      tasks:
        - name: "inldue role"
          include_role:
            name: role_ansible_clone_git_repo
          vars:
            git_repo_url: <repo url>
            branch: <repo branch to clone>
            clone_dest_path: <full destination path to clone the repository>
            bb_username: < username >
            bb_password: < password >


Testing Platform
----------------

- Red Hat Enterprise Linux Server release 7.6 (Maipo)

Author Information
------------------

- Yasin Faizan S MD
