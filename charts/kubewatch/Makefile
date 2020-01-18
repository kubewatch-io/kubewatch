NAME := kubewatch 
OS := $(shell uname)

build: clean
	helm lint
	helm template .

lint: clean
	helm lint
	helm template .

install: clean build
	helm install . --name ${NAME}

upgrade: clean build
	helm upgrade ${NAME} .

delete:
	helm delete --purge ${NAME}

clean:
	rm -rf charts
	rm -rf ${NAME}*.tgz

release: clean build
	helm package .
	rm -rf ${NAME}*.tgz
