# ansible-roles-roboshop
It is a demonstration ansible roles, how we can use in industries

Ansible Roles: It is a proper directory structure to write ansible palybooks, we can reuse roles.

Template-> We can keep some placeholders, you can put the vaues at run time.
we cna reuse those templates in future.

file --> content inside a specific file

ansible template:- It follows jinja2 formatting, we can keep some placefolders, actual values will be provided thorough variables at runtime.

tasks
   main.yaml  --> playbook related tasks are here
files
    <file-name> --> you can keep all the files reuired here

templates
    <templates-file> --> we can keep all the templates with placeholders here. usually we follow jinja2 templating, variables values can be supplied.
vars
    main.yaml --> we can keep all the vars here
 
 Handlers --> these are notifiers in ansible. When there is a change in something if you want to notify oyhrt task we can use handlers.
 we can usee handlers properly for restarting the servers or services when any configuration changes happend.
 Eg:- change in nginx configure can notify restart task in handlers directory.
   <some-name>.yaml




Ansible Tag:-
==============================================
Use case--> If you want to run some specific tasks in ansile we use Ansible Tags to run that specific tasks.


We can include other roles using include_role or import_role

Include_role: it will include tasks in run time and it also validates during runtime only

Import_role: Ansible validates the import_role before execution of playbook
Tags and when conditions apply to the imported role and its tasks.
   