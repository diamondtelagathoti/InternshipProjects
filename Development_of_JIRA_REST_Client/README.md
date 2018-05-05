# JIRA REST Client

Developed a _REST Client_ which extracts the Bug Report from the database first and log all the _Bug Reports_ with relevant stats to specific JIRA Project using REST API provided by JIRA.  

#### Installation:

* Run the following command to install all the packages:  
	``sudo pip3 install -r packages.txt``  
	``sudo apt-get install python3-pandas``  

For more information on installing dependencies, refer the link:  
[Installation of JIRA](https://jira.readthedocs.io/en/master/installation.html)  

* To check whether JIRA is installed successfully or not:  
Open the terminal:  
``
	python3
	from jira import JIRA
``

#### Code Example:

* After installing all the dependencies, supply the following command as the program has a command line interface.  
	``python3 jira_rest_client.py -dbname databasename -hname hostname -u username -p password``  

* There are 4 arguments which you must pass as a command line argument, which are:  
1. -dbname: Name of the database.  
2. -hname: Hostname of the database.  
3. -u: username of the database.  
4. -p: password of the database.  

``E.g. python3 jira_rest_client.py -dbname localhost -hname 127.0.0.1 -u abcdef -p 12345678``  

#### References:
* For more information on _How The REST Client Works_, refer the link:  
[How The REST Client Works](https://docs.google.com/document/d/1CHUcDlvIS7zXKYXRY1dFw2VWpx4xE4YB63O0jG0dfM8/edit?usp=sharing)  

* For more information on _Python JIRA REST API_, refer the link:  
[Python JIRA REST API](https://jira.readthedocs.io/en/master/api.html)  

