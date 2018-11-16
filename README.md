# Matrix
Collaboration Matrix is a visualization showing the connectedness and collaboration between authors and their affiliations. Visit https://rin.lipi.go.id/matrix/ to play with a production installation.

**The "Content of Relations"** dropdown is used to select the contents of matrix collaboration content. There are 2 choices of content, namely:

1. Based on Author = displays a collaboration matrix between the author name.
2. Based on Affiliation = displays a collaboration matrix between affiliation.

**The "Order by"** dropdown is used to sort the appearance of the matrix. There are 4 types of order choices, namely:

1. Name (A-Z) = sort by alphabetical order name.
2. Highest Frequency = sort by the highest collaboration frequency.
3. Count Per Name = sort by number of collaborations per name.
4. Leaf Order = sort by proximity of collaboration values per name.

The first 25 collaborations are displayed.


### Minimum Requirement :
- Glassfish 4
- Java JDK 8
- PostgreSQL 9.2

### Test Deploying an Application From the Command Line

1.	To download a copy of the 'matrix.war' application.
2.	Save the matrix.war file in the directory of your choice. This directory is referred to as *sample-dir*.
3.	Start Glassfish Server domain before deploy the application. To Start the Default Domain. Run the asadmin start-domain command without an operand: 

    **as-install/bin/asadmin start-domain**

    The command starts the default domain, domain1.

4.	Use the asadmin deploy command. General command is: 

    **as-install/bin/asadmin deploy war-name**

    To deploy the matrix.war sample, the command is:

    **as-install/bin/asadmin deploy sample-dir/matrix.war**
    
    Normally can be create in */domain1/applications/matrix/*

5.	Access the matrix application by typing the following URL in your browser:

    **http://localhost:8080/matrix**
    
6.	The application's start page is displayed.

See Full Documentation Glassfish : [Doc Glassfish 4](https://javaee.github.io/glassfish/doc/4.0/quick-start-guide.pdf).



### Config Database
Configure Script To Connect Database PostgreSQL Server in File "config.json" at */matrix/resources/data/config.json*

Example Default Config :

![2018-08-16_00h42_36](https://user-images.githubusercontent.com/42184550/44163344-521b1500-a0ed-11e8-8fe4-0da3583b3b94.png)

- host = "IP database PostgreSQL server"
- port = "port database"
- dbname = "the name of database"
- username = "username to access database"
- password = "password to access database"
- pathjsonfile = "folder location where json file is stored" *(normally it doesn't need to be changed)*





### Examples Output Matrix :
![2018-08-16_15h30_11](https://user-images.githubusercontent.com/42184550/44197598-4a00bb00-a169-11e8-86eb-c08f22add5a7.png)

![2018-08-16_15h29_48](https://user-images.githubusercontent.com/42184550/44197607-4ff69c00-a169-11e8-9acc-bb78bf8808c5.png)



