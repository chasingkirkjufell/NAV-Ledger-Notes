# NAV-Ledger-Notes

Using Ledger NavCoin App on a Ubuntu 18.04 VM with VirtualBox on Windows 10 Pro

Some steps may not be needed but these are the steps that I took and it worked

git clone https://github.com/aguycalled/electrum --branch nav

sudo apt-get install python3-pyqt5

sudo apt-get install pip

sudo apt-get install libusb-1.0-0-dev

sudo apt-get install libudev1 libudev-dev

sudo apt-get install python3-setuptools

python3 -m pip install .[fast]

wget -q -O - https://raw.githubusercontent.com/LedgerHQ/udev-rules/master/add_udev_rules.sh | sudo bash

Followed instructions here: https://github.com/aguycalled/ledger-app-nav/releases/tag/317

Remember to download the assets and put them in a folder and run the commands in that folder. I justed just downloaded the assets to the cloned electrum folder and ran everything there.

And in the cloned electrum folder.

python3 setup.py build

python3 run_electrum

Eletrcum wallet should start now. In one of the steps of creating a wallet, you can choose using a hardware wallet and then legacy address.
