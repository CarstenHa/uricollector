# Linux install example

## Install into a virtual environment

    git clone https://github.com/CarstenHa/uricollector
    python3 -m venv /path/to/uricollector
    cd /path/to/uricollector
    source bin/activate
    bin/pip install requests
    bin/pip install googlesearch-python
    deactivate

## Upgrade VE (e.g. after Linux Release-Upgrade)

    # Upgrade VE
    python3 -m venv --upgrade /path/to/uricollector
    cd /path/to/uricollector
    # Update uricollector
    git pull
    # Upgrade packages
    source bin/activate
    bin/pip install -U requests googlesearch-python
    deactivate
