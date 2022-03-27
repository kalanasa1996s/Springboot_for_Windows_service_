# Springboot_for_Windows_service_
Create windows service for spring boot using winsw

1).Download WinSW and rename exe file WinSw.exe 
  
      https://github.com/winsw/winsw/releases
      
2).Create xml file and rename WinSw.xml and inlcud configurations

      
      <configuration>
      <!-- ID of the service. It should be unique across the Windows system-->
      <id>serviceName</id>
      <!-- Display name of the service -->
      <name>MyApp Service (powered by WinSW)</name>
      <!-- Service description -->
      <description>Spring boot app running as Win service</description>
  
      <!-- Path to the executable, which should be started -->
      <executable>java</executable>
      <arguments>-jar %BASE%\springpro.jar</arguments>

      </configuration>

3). Create Folder --> and file inclued jar file ,xml and exe 

4). Open cmd and type 
    
    winsw install FolderPath
    winsw run folder path
    
    
    
    
* https://github.com/winsw/winsw/blob/v3/docs/cli-commands.md#install-command
      
      
