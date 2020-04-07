Using NS-3 and NSAnim, CupCarbon as the tools.


### The process of install CupCarbon

The application is based on JDK 11.
  1. Install JDK 11 at first.
    Using "java -version" to check if it was installed successfully
  2. Becaust Oracle removed ```javafx``` in JDK 11, we need to install in Ubuntu.
    Download .zip from (https://gluonhq.com/products/javafx/)
    Unzip the .zip file.
    Copy all the files in the lib folder to the lib folder of JAVA_HOME by using---
   
    
    cd javafx-sdk-11.0.1
    
    sudo cp -arf lib/* ${JAVA_HOME}/lib/
  
  
  3. List the javafx library location using below command

    $ dpkg-query -L openjfx
    
  4.  Run the jar application
  
    java --module-path //home/pwrs/Downloads/javafx-sdk-11.0.2/lib  --add-modules=javafx.controls,javafx.fxml,javafx.base,javafx.media,javafx.web,javafx.swing -jar '/home/pwrs/cupcarbon.jar'
    
    
 Reference: https://ayaztechy.blogspot.com/2019/09/cupcarbon-iot-simulator-installation-in.html
