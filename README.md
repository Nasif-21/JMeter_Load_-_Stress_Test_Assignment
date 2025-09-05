# Load and Stress Test for a server using JMeter
This project contains stress and load test on a book shop app to find out how it performs under stress and finding the limit to handle request on a secnario.

## Technical Requirement:
+ Apache JMeter
+ Java JDK and environment setup
+ Java
+ Git command

## Pre Requisits
+ Download Apache JMeter into your PC
+ Download the JAVA JDK (LTS version highly preferable)

## Set Up the environment:
+ First download the JAVA JDK, install in a folder and set up path and home variable
+ Download JMeter and install on a folder
+ Run the JMeter on double click on ApacheJMeter.jar. Another way is, open command prompt and write ```jmeter``` to run Apache Jmeter

## Performing Tests:
+ clone this repository to your pc and put into a folder
+ Open JMeter and Go to File>Open>``booking.jmx``
+ Inside tread group, you will see Number of threads(user) and Ramp-up-preiod.
+ Based on the throuput, increase time and numbers of user
+ On Summary report, you can see how its performing on current thread.
+ If there is an error while performing, increase ramp up preiod on that perticular thread/user

## Running Reports and JMeter Dashboard
+ Go to the file where ``booking.jmx`` file is stored.
+ Open command line
+ Write this command : ```jmeter -n -t .\booking.jmx -l .\booking.jtl -e -o Reports```
+ An report folder, jmeter log and jtl file will be created
+ Under report folder, there is an html file name index, open to view the reports


## Attachments:
### JMeter Dashboard screenshot:
<img width="1915" height="896" alt="image" src="https://github.com/user-attachments/assets/97a4ece0-9c30-415f-a8b6-b3eead68bf5d" />

### Load Test report screenshot:
<img width="1919" height="1013" alt="image" src="https://github.com/user-attachments/assets/42725c66-45fd-4529-b7b2-aaf8e12d0831" />

### Stress Test report screenshot:
<img width="1919" height="1019" alt="image" src="https://github.com/user-attachments/assets/e98ff929-d8e2-4c10-9ccf-98952a861098" />


