# Configuring a Raspberry Pi

Assumes you're using Raspbian Jessie  with Pixel or newer.

## Ansible Configuration

### Command Examples

Assuming you are in the `inventories` directory of this project when running from the terminal.

#### Basic Ping Test Using Ansible Command Line

`ansible pis -i tinkurpi -m ping -u pi --ask-pass`

#### Basic Ping Test Using An Ansible Playbook

Simulate Running the Playbook

`ansible-playbook setup_pi.yaml -s -C -i tinkurpi --ask-pass`

Running the Playbook

`ansible-playbook setup_pi.yaml -s -i tinkurpi --ask-pass`

### Playbook to Configure Pi

Running the Playbook

`ansible-playbook setup_pi.yaml -s -i tinkurpi --ask-pass`

## Dashboard Configuration

[List](http://peter.sh/experiments/chromium-command-line-switches/) of Chromium Command Line Switches.

### Launch Chromium Browser in Kiosk Mode w/ URL
`chromium-browser URL URL URL --kiosk`

### Exit Chromium Browser
`Ctrl + W`





