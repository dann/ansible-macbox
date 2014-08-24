.PHONY: default all setup check
default: all

all: setup

setup: check
	ansible-playbook -K ./site.yml

setup_simple:
	ansible-playbook -K ./site.yml --skip-tags "homebrew"

check:
	ansible-playbook -K ./site.yml --syntax-check

facts:
	ansible -m setup localhost
