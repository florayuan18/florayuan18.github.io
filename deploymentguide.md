---
layout: page
title: Deployment Guide
subtitle: Maggie Killada
---
## Materials
- Raspberry Pi (Raspberry Pi 400 Unit Keyboard) _this is the hardware we will use_
- VNC Viewer (on both Pi and on host)
- Monitor
- Keyboard & Mouse

## Using Raspberry Pi
1. connect power source
2. connect mouse through USB port
3. connect to monitor to view through an HDMI cable
4. power up the pi, login and get setup

## Using VNC Viewer
1. create account on personal computer
2. download VNC Viewer on personal computer and on the Raspberry Pi
3. in VNC Viewer application, select "computers" from the sidebar and then select the raspberry pi computer (Name: raspberrypi)

## Setting up Java web on Raspberry Pi
In terminal:
1. install necessary packages\
   `sudo apt install & sudo upgrade`\
   `sudo apt install default-jre default-jdk maven`
2. clone the repository\
   `cd` for navigating files and `cd~` to navigate to home directory\
   `git clone https://github.com/florayuan18/pikachudrinkingwindex.git`
3. run the repository\
   `cd pikachudrinkingwindex`\
   `sudo mvn spring-boot:run`
4. test site on Raspberry Pi browser (Chromium) using "localhost:8080"

## Creating a service on Raspberry Pi
Execute these lines in terminal:
1. `cd /etc/systemd/system/`
2. `sudo touch AllHailTheHolyScrumMaster.service`
3. `sudo systemctl start AllHailTheHolyScrumMaster`
4. `sudo systemctl status AllHailTheHolyScrumMaster`
5. `cd /etc/nginx/sites-available`
6. `sudo touch AllHailTheHolyScrumMaster`
7. `sudo ln -s /etc/nginx/sites-available/AllHailTheHolyScrumMaster /etc/nginx/sites-enabled`
8. `sudo nginx -t`
9. `sudo systemctl restart nginx`

## Creating a custom domain name using Freenom
1. head to freenom.com
2. make a Freenom account (Recommend personal google account)
3. create a new domain
4. choose between (recommend .cf)
5. once domain is created head over to "services"
6. click my domains
7. click "Manage Domain"
8. then click on "Manage Freenom DNS"
9. head to "Register glue records"
10. obtain your external IP address using "What is my IP Address"\
    ![freenom.png](https://github.com/florayuan18/pikachudrinkingwindex/blob/master/src/main/resources/static/images/freenom.png)

## Port forwarding
1. login to home router app/web
2. setup your router to forward TCP/UDP to raspberry pi server
3. start your raspberry pi server using the sudo command
4. Use sudo command to thonny (run this or you may get some errors when running your website on multiple devices)
5. check to make sure that you have port 80
6. test your website on any browser

## Update Deployment
1. navigate to directory\
   `cd` to default and `cd pikachudrinkingwindex` to navigate to project
2. update the repository\
   `git pull`
2. update procedures\
   `./mvnw package`\
   `sudo systemctl restart pikachudrinkingwindex.service`

### Sources:
* https://csa.nighthawkcodingsociety.com/course/deploy
* https://docs.google.com/presentation/d/1-afmt3XGlzlVqjwS8Ign6y61j-st1VhoFk3uwW3o6Sk/edit?usp=sharing
* https://github.com/nighthawkcoders/nighthawk_csp
* https://github.com//nighthawkcoders/nighthawk_csa
* https://docs.google.com/document/d/1nODveWp0jBzj4ZpFLgWCWTOXzLAHAPUhAQYmZJ4LhyU/edit?usp=sharing