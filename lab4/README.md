
# Lab 4 - Setting up App Insights (AI) in VS Code
In this lab we will walk through adding an  Application Insights framework to a sample  Node.js/Express project. We will also showcase the tight AI/VS Code integration that will enable more agile development process by providing real-time AI telemetry (CodedLens) feedback in the IDE.  

## Create a sample Node.js Express project
Initialize a node application (pick defaults)
``` bash
npm init
```
Boostrap the Express framework (pick defaults and agree to overwrite the destination by typing 'y')
``` bash
express
```
The output will look similar to this:

![express](/images/lab4-express.png)

## Install an App Insights extension in VS Code
Open Visual Studio Code and install the Application Insights extension. You can use the command line shortcut if your PATH is configured ([more details](https://code.visualstudio.com/docs/setup/setup-overview)).
```bash
code .
```
Navigate to the Extensions tab, search and install the Azure Application Insights

![AI Extention](/images/lab4-ai-ext.png)

## Deploy an App Insights resource in Azure
## Add AI to the project and connect to Azure
In VS Code bring up the command pallete by using the menu or command line shortcut: Ctr+Shift+P (Windows) or Command+Shift+P (Mac).

![Command Pallete](/images/lab4-vscode-ai.gif)
## View the code telemetry using CodeLens
## View the code telemetry in the AI portal

