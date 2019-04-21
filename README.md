# RoR2Mods
i dont know what im doing  
this repo is likely to be outdated compared to its submodules so navigate each one seperately for updates/releases _(make sure to use master branch)_

# Boilerplate
this repo has a solution that uses `Directory.Build.targets` to automatically link projects with installed assemblies (i.e. you have to have bepinex installed before you open solution and try to build it)  
it will try to find the location of risk of rain 2 based on the registry for both the game and steam  
right now its at windows only but if i see an interest to get it to work with others, i might change it

## "Failed to find RoR2 install path"
create a new file named `Directory.Build.targets.user` in the same folder as the solution file and paste the following:
```xml
<Project xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
   <PropertyGroup>
     <GamePath>PATH_HERE</GamePath>
   </PropertyGroup>
</Project>
```
replacing `PATH_HERE` with path to Risk of Rain 2

# Mods
currently there's only one  
i dont know if there's going to be more
