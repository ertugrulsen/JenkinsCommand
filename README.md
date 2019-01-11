"# JenkinsCommand" 

Build Command
C:\Jenkins\workspace\TeknosaLive51\WebSite.sln
-------------------------------------------------------
/t:Build /p:VisiualStudioVersion=14.0 /property:Configuration=Release /p:DeployOnBuild=True  /p:UserName=**** /p:Password=*** 
/p:AllowUntrustedCertificate=True /p:MSDeployPublishMethod=WMSVC 

-------------------------------------------------------------------------------
/t:Build /p:VisiualStudioVersion=14.0 /property:Configuration=Release /p:DeployOnBuild=True /p:PublishProfile=JenkinsLiveProfile /p:UserName=*** /p:Password=** 
/p:AllowUntrustedCertificate=True /p:MSDeployPublishMethod=WMSVC 

#####Deploy for IIS#####
cd C:\Program Files\IIS\Microsoft Web Deploy V3
msdeploy.exe -source:package='***.zip' -dest:auto,computerName=***/msdeploy.axd?site=***,userName=***,password=***,authType=basic -verb:sync -setParamFile:"****.SetParameters.xml" -allowUntrusted






