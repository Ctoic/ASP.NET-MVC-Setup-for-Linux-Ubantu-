# ASP.NET-MVC
# Introduction 
  1. It was introduced in 1970.
  2. It is widely used to create web apps
  3. It is similar to ruby on rails and express for Node.
  4. Asp.net mvc is an open source software from Microsoft.
  5. The web development framework combines the feature of MVC(model-view-Control) architecture and the most up to date agile development and the best parts of the existing Asp.net platform.

## Preuisites 
1. You should know the Basics of C# 
2. Familiar with Visual Studio on windows and for Lilnux user should know Rider.
## MVC 
a). Model : Application data and behaviour in terms of its problem domain and independent of UI.
b). View : The HTML markup displayed to the user
c). Controller : Responsible for all our HTTP request handling.
d). Router: Select the right controller.


![1200px-MVC-Process svg](https://user-images.githubusercontent.com/90936436/198706350-886f93aa-865f-4b71-b966-7d1c394338cf.png)

For example if we want to create a web application named as bugdetector then we will have the following HTTP: http://bugdetector.com/blog when we send a request to this http a controller is selected to handle this request. Then It will communicate with database to collect the related information(Model) and Finally return the view to the client or browser(View).


# Setting up the Envirement on Ubantu(Linux)
<div>
  <h3>what is OBDC?</h3>
  <p> 
  Open Database Connectivity (ODBC) is an open standard Application Programming Interface (API) for accessing a database. In 1992, Microsoft partners with Simba to build the world’s first ODBC driver; SIMBA.DLL, and standards-based data access was born. By using ODBC statements in a program, you can access files in a number of different common databases. In addition to the ODBC software, a separate module or driver is needed for each database to be accessed.</p>
  </div>
<div>
<h1>This article provides commands for installing the ODBC driver from the bash shell. If you want to download the packages directly</h1>
<p>
  
    if ! [[ "18.04 20.04 22.04" == *"$(lsb_release -rs)"* ]];

    then
  
    echo "Ubuntu $(lsb_release -rs) is not currently supported.";
    
    exit;

     fi
  
</p>

<p>
  
  $ sudo su
  
    curl https://packages.microsoft.com/keys/microsoft.asc | apt-key add -

    curl https://packages.microsoft.com/config/ubuntu/$(lsb_release -rs)/prod.list > /etc/apt/sources.list.d/mssql-release.list

    exit
  
    $ sudo apt-get update
  
  
    $ sudo ACCEPT_EULA=Y apt-get install -y msodbcsql18

  
  ## optional: for bcp and sqlcmd
    $ sudo ACCEPT_EULA=Y apt-get install -y mssql-tools18
  
    echo 'export PATH="$PATH:/opt/mssql-tools18/bin"' >> ~/.bashrc
    
    $ source ~/.bashrc
  
### optional: for unixODBC development headers

  
      $ sudo apt-get install -y unixodbc-dev

  </p>
</div>

<div>
  <h3>Download and Install AzureDataStudio</h3>

  <p>Azure Data Studio is a cross-platform database tool for data professionals using on-premises and cloud data platforms on Windows, macOS, and Linux.

Azure Data Studio offers a modern editor experience with IntelliSense, code snippets, source control integration, and an integrated terminal. It's engineered with the data platform user in mind, with built-in charting of query result sets and customizable dashboards.

The source code for Azure Data Studio and its data providers is available on GitHub under a source code EULA that provides rights to modify and use the software, but not to redistribute it or host it in a cloud service.
    
**DownloadAzureStudio** 🔗https://go.microsoft.com/fwlink/?linkid=2204570

  </p> 
<h2>Installing On Linux</h2>
<div>

1. write the following command on the terminal.
  
                $ sudo dpkg -i ./Downloads/azuredatastudio-linux-<version string>.deb 

  2. Run this and Azurestudio will open.
  
              $ azuredatastudio

<h2> It provides You</h2>
    <p>
    
        1. SQL code editor with IntelliSense 
        2. Smart SQL code snippets
        3. Customizable Server and Database Dashboards
        4. Connection management (server groups)
        5. Integrated Terminal
        
        
     </p>



</div>
