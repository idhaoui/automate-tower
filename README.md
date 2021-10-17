
Original source : https://github.com/redhat-cop/automate-tower

The steps to use it are relatively simple:

. `cp tower-setup-inventory.example.yml tower-setup-inventory.local.yml`
. adapt this new inventory file to your needs
. call the playbook `tower-setup.yml`, e.g. with something like `ansible-playbook -i tower-setup-inventory.local.yml tower-setup.yml -v`

Check the README.md file of the role for more information and more variables to use to steer the role.

NOTE: the temporary directory isn't cleaned, so you might want to do it once everything looks fine.
