After adding the 127.0.0.1 ci.kbase.us line in /etc/hosts and changing the following lines in Makefile:

#NODE_REQUIRED="v6"
NODE_REQUIRED="v8"

run the following commands:
--------------------------------
cd kbase-ui
make init; make build; make dev-image; make run-dev-image
--------------------------------

where 'make init' only needs to run once, while 'make build; make dev-image; make run-dev-image'
can be run as many times as needed to test my changes

Once make run-dev-image is running, I can go to the browser and type in 'ci.kbase.us' to see my
changes in effect.
