# Configuring a Raspberry Pi

Assumes you're using Raspbian Jessie  with Pixel or newer.

## Ansible Configuration

### Command Examples

Assuming you are in the `inventories` directory of this project when running from the terminal.

#### Basic Ping Test Using Ansible Command Line

`ansible pis -i tinkurpi -m ping -u pi --ask-pass`

#### Basic Ping Test Using An Ansible Playbook

Simulate Running the Playbook

`ansible-playbook ../playbooks/setup_pi.yaml -s -C -i tinkurpi --ask-pass`

Running the Playbook

`ansible-playbook ../playbooks/setup_pi.yaml -s -i tinkurpi --ask-pass`

### Playbook to Configure Pi

`ansible-playbook ../playbooks/setup_pi.yaml -s -i tinkurpi --ask-pass`

## Dashboard Configuration

[List](http://peter.sh/experiments/chromium-command-line-switches/) of Chromium Command Line Switches.

### Launch Chromium Browser in Kiosk Mode w/ URL at Startup
In `~/.config/lxsession/LXDE-pi/autostart` add `@chromium-browser URL URL URL --kiosk`

See [Autostart reference](https://wiki.archlinux.org/index.php/LXDE#Autostart) for all commmands.

### Exit Chromium Browser
`Ctrl + W`

## To Do

Run Python script
Add `@/usr/bin/python /home/pi/example.py`






