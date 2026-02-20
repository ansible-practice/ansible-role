(in progress)


ssh to azure vm -- > 
            ssh -i azure_key.pem azureuser@20.234.37.129

            sudo apt update

Install ansible on the vm --> 
            sudo apt install ansible

Check ansible version --> 
            ansible --version

Create dummy ansible role for practice --> 
            ansible-galaxy role init ansible-practice

Do changes in vs code --> 

open remote window in vs code and ssh to the vm.

update the config based on pem file location -->

    Host ansible-control
        HostName 20.234.37.129
        User azureuser
        IdentityFile ~/.ssh/ansible-practice-vm_key.pem
        IdentitiesOnly yes
