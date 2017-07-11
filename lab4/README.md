# Lab 4 - Setting up App Insights (AI) in VS Code

In this lab we will walk through adding an  Application Insights framework to a sample  Node.js/Express project. We will showcase the AI/VS Code integration that will enable more agile development process by providing real-time AI telemetry (CodeLens) feedback in the IDE and the portal.

## Create a sample Node.js Express project

Initialize a node application (pick defaults)

``` bash
npm init
```

Bootstrap the Express framework (pick defaults and agree to overwrite the destination by typing 'y')

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

![AI Extension](/images/lab4-ai-ext.png)

## Add AI to the project and connect to Azure

In VS Code bring up the command palette by using the menu or command line shortcut: Ctr+Shift+P (Windows) or Command+Shift+P (Mac) and select "Application Insights: Add To Project"

![Command Palette](/images/lab4-vscode-ai.gif)

Select "Add Account" and follow the login instructions (if not already logged in). If you are logged in, select you account from the drop down.

![AI Login](/images/lab4-ai-account.png)

Once logged in VS Code will prompt you to select a subscription and a resource group.

Finally, VS Code will add the required npm package to node_modules folder, add a config file **aisettings.json** containing the AI key and will bootstrap the required code in the app.js.

You should immediately start seeing the telemetry annotations in your code (more details below).

## View the code telemetry using CodeLens

Once the AI SDK is installed and bootstrapped, navigate to your controller (index.js in our case) and notice the AI CodeLens annotations above each route. You can see some quick statistics about the number of requests, failures and average response time. Click on the annotation to get additional details.

![AI CodeLens](/images/lab4-ai-telemetry-ide.png)

## View the code telemetry in the AI portal

You can also go a level deeper by viewing the AI telemetry in the Azure portal (click on the App Insights icon in the IDE).

![AI Portal](/images/lab4-ai-telemetry-portal.png)
