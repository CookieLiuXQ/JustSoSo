#### 	 dotnet ref

##### 	nuget

1.  nupkg create

   ```	
   <Project Sdk="Microsoft.NET.Sdk">
     <PropertyGroup>
       <Description>Provides access to the mongo database client.</Description>
       <AssemblyTitle>xxxxx</AssemblyTitle>
       <VersionPrefix>2.2.0</VersionPrefix>
       <Authors>Me</Authors>
       <TargetFramework>netstandard2.0</TargetFramework>
       <AssemblyName>xxxxx</AssemblyName>
       <Description>Provides access to the mongo database client.</Description>
       <PackageId>xxxxx</PackageId>
       <PackageTags>metadata;mongodb;driver</PackageTags>
       <PackageReleaseNotes>Update MongoDB.Driver to 2.15.1</PackageReleaseNotes>
       <RepositoryType>git</RepositoryType>
       <RepositoryUrl>https://xxxxx</RepositoryUrl>
       <GenerateAssemblyConfigurationAttribute>false</GenerateAssemblyConfigurationAttribute>
       <GenerateAssemblyCompanyAttribute>false</GenerateAssemblyCompanyAttribute>
       <GenerateAssemblyProductAttribute>false</GenerateAssemblyProductAttribute>
     </PropertyGroup>
   ...
   ```

   then   

   1.  right click the project to [package]
   2.  go to the directory [program->src->main project->bin->release] and you will see xxxx.nupkg there   



2.  nupkg upload  



   1.  open [cmd] in the [release] directory and upload the xxxx.nupkg

      ```
      dotnet nuget push xxxxx.2.2.0.nupkg --api-key xxxxxxxx --source http://xxxxxx/
      ```

      PS: 

      1.   --api-key   the authorize param     cli followed to set the key to the specific address for the first time and after that you can push to the address without the key 

      2.   --source the address  nupkg upload to 

         ```
         dotnet nuget setapikey xxxxxxx -source http://xxxxxx/
         ```

         

      

