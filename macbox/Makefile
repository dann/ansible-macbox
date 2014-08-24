.PHONY: default all clean build run deploy save_deps
default: all

all: setup

setup:
	ansible-playbook -K ./site.yml

setup_simple:
	ansible-playbook -K ./site.yml --skip-tags "homebrew"
