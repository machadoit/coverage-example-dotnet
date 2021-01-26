# Coverage example on dotnet core

- ```docker run -it -v $(pwd):/src  mcr.microsoft.com/dotnet/sdk:5.0```
- Install dotCover on the docker in any folder, example on installing `2020.3.2`:
    - ```wget https://download.jetbrains.com/resharper/dotUltimate.2020.3.2/JetBrains.dotCover.CommandLineTools.linux-x64.2020.3.2.tar.gz```
    - ```tar -zxf JetBrains.dotCover.CommandLineTools.linux-x64.2020.3.2.tar.gz```
- On the `/src` folder run:

    - ```<path-where-unpacked-dotCover>/dotCover.sh dotnet --output=dotcover.xml --reportType=DetailedXml -- test```
