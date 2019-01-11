"# JenkinsCommand" 

Build Command
-------------------------------------------------------
/t:Build /p:VisiualStudioVersion=14.0 /property:Configuration=Release /p:DeployOnBuild=True  /p:UserName=**** /p:Password=*** 
/p:AllowUntrustedCertificate=True /p:MSDeployPublishMethod=WMSVC 

-------------------------------------------------------------------------------
/t:Build /p:VisiualStudioVersion=14.0 /property:Configuration=Release /p:DeployOnBuild=True /p:PublishProfile=JenkinsLiveProfile /p:UserName=*** /p:Password=** 
/p:AllowUntrustedCertificate=True /p:MSDeployPublishMethod=WMSVC 

#####Deploy for IIS#####
cd C:\Program Files\IIS\Microsoft Web Deploy V3
msdeploy.exe -source:package='***.zip' -dest:auto,computerName=***/msdeploy.axd?site=***,userName=***,password=***,authType=basic -verb:sync -setParamFile:"****.SetParameters.xml" -allowUntrusted


Jenkins Jmeter Command

C:\Users\ertugrul.sen\Desktop\apacheJmeter\apachejmeter4.0\bin\jmeter.bat -jmeter.save.saveservice.output_format=xml -n -t C:\Users\ertugrul.sen\Desktop\apacheJmeter\LoginScript.jmx -l Test.jtl



