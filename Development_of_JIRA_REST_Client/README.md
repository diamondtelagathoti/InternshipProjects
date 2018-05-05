# JIRA REST Client

Developed a _REST Client_ which extracts the Bug Report from the database first and log all the _Bug Reports_ with relevant stats to specific JIRA Project using REST API provided by JIRA.  

#### Installation:

* Run the following command to install all the packages:  
	``sudo pip3 install -r packages.txt``  
	``sudo apt-get install python3-pandas``
* After installing all the dependencies, supply the following command as program has a command line interface.  
	``python3 jira_rest_client.py -dbname databasename -hname hostname -u username -p password``  

For more information on _How The REST Client Works_, refer the link:  
[How The REST Client Works](https://docs.google.com/document/d/1CHUcDlvIS7zXKYXRY1dFw2VWpx4xE4YB63O0jG0dfM8/edit?usp=sharing)  

For more information on _Python JIRA REST API_ refer the link:  
[Python JIRA REST API](https://jira.readthedocs.io/en/master/examples.html)  

