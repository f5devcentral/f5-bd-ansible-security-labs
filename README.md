# f5-bd-ansible-security-labs

Updated for Event-Driven Automation code, This will test out Event Driven Automation Security lab with RedHat Event Driven Ansible

This code is free to use

Directory Structure 

- elastic-watcher - contains code used for elastic watcher that triggers webhook for Anible-Rulebook.  
    - **Note** I had to convert from its XML to JSON format to make the watcher work correctly with EDA, but this shows a good example of how to inject payloads and convert the XML output to JSON.
- f5-playbooks - these are the playbooks being executed by the ansible-rulebook code
    - **Note** there is a bug in the Ansible-Rulebook code that has been committed and just waiting for it to be merged in the main code stream. see code https://github.com/ansible/ansible-rulebook/issues/508 (Issue was found in v0.13.0)
- rulebooks - these are the rulebooks that create the webhook watcher and execute when the message from the webhook matches.
- testing-playbook - these are other playbooks i used to validate code function not needed for this code but just good to know

