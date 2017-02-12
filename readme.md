# Configuring a Raspberry Pi

Assumes you're using Raspbian Jessie  with Pixel or newer.

## Ansible Configuration

### Command Examples

#### Basic Ping Test Using Ansible Command Line

`ansible pis -i /Users/adamzolyak/Documents/Source/ansible/inventories/tinkurpi.ini -m ping -u pi --ask-pass`

#### Basic Ping Test Using An Ansible Playbook

Simulate Running the Playbook
`ansible-playbook setup_pi.yaml -s -C -i /Users/adamzolyak/Documents/Source/ansible/inventories/tinkurpi.ini --ask-pass`

Running the Playbook
`ansible-playbook setup_pi.yaml -s -i /Users/adamzolyak/Documents/Source/ansible/inventories/tinkurpi.ini --ask-pass`

### Playbook to Configure Pi

Running the Playbook
`ansible-playbook setup_pi.yaml -s -i /Users/adamzolyak/Documents/Source/ansible/inventories/tinkurpi.ini --ask-pass`

## Dashboard Configuration

[List](http://peter.sh/experiments/chromium-command-line-switches/) of Chromium Command Line Switches.

### Launch Chromium Browser in Kiosk Mode w/ URL
`chromium-browser URL URL URL --kiosk`

### Exit Chromium Browser
`Ctrl + W`





