
java -jar "NapBrowser.jar" 

Linux:
1. install  java min. 8

2. If toolkit error:
https://askubuntu.com/questions/695560/assistive-technology-not-found-awterror
Description:
This can be done by editing the accessibility.properties file for OpenJDK 8 (change the version to whichever is actually in use on your system):
sudo vim /etc/java-8-openjdk/accessibility.properties
Comment out the following line:
#assistive_technologies=org.GNOME.Accessibility.AtkWrapper

3. If libgconf-2-4 error:
https://support.circleci.com/hc/en-us/articles/360004086734-error-while-loading-shared-libraries-libgconf-2-so-4-cannot-open-shared-object-file-No-such-file-or-directory?utm_medium=SEM&utm_source=gnb&utm_campaign=SEM-gnb-DSA-Eng-ni&utm_content=&utm_term=dynamicSearch-&gclid=EAIaIQobChMIvoOB_fnj7AIVRht7Ch1W0QulEAAYASAAEgIGPPD_BwE
sudo apt-get install libgconf-2-4
