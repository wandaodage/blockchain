Step1: Prepare development environment
================

###
	yum install gcc openssl-devel bzip2-devel
### 
	cd /usr/src
### 	
	wget https://www.python.org/ftp/python/3.6.4/Python-3.6.4.tgz
###  
 	tar xzf Python-3.6.4.tgz
### 
	cd Python-3.6.4
###  
	./configure --enable-optimizations
###  
 	make altinstall
###  
 	pip3.6 install pipenv
###  
	pipenv --python=python3.6
###  
	pipenv install requests
###  
 	pipenv install flask

Step2: Create blockchain.py
=================

###
	mkdir blockchain
###  
	cd blockchain/
###  
	touch blockchain.py
###  
 	chmod +x blockchain.py

Step3: Run blockchain service
=================

Open two terminal, run below commands seperaterly

###
	pipenv run python blockchain.py -p 5001
###
	pipenv run python blockchain.py -p 5002



