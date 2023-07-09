# Azure Function-App-Calculator
- Using Http Trigger to call an Azure-Function-App that sums the value of x and y and inputs a result
- The app is run locally and also published to Azure 
- The class was renamed to sum
- The function attribute was also renamed to sum
- The content of run method was deleted
- The logger was not deleted
- Lines as shown below were added 
- int x =int.Parse(req.Query["x"]); line 22
- int y =int.Parse(req.Query["y"]) line 23
- int result = x + y line 24
  return new OkobjectResult(result); line 25
- The parseInt method parses a value as a string and returns the first integer
## Creating-Azure-Function-App  
- Azure Functions lets you run your code in a serverless environment without having to first create a virtual machine (VM) or publish a web application
- Sign in to the Azure portal with your Azure account
- In the search bar, enter Function App and CreateOn the Basics page, use the function app settings as specified in the following *Function App name- calculatortests and others at default with your proper Region selected
- On the Hosting page, enter the following settings. *Operating system- Windows *Plan- Consumption (Serverless-In this serverless hosting, you pay only for the time your functions run)
- Select "Review + create" to review the app configuration selections.
On the "Review + create" page, review your settings, and then select "Create" to provision and deploy the function app
- Select "Go to resource" to view your new function app. You can also select Pin to dashboard. Pinning makes it easier to return to this function app resource from your dashboard
## Deploying From Visual Studio to Azure  
- Search for "Publish" Select Azure / Right-click on the project in Solution Explorer and select "Publish"
- Then select "Azure function App (windows)" Click Next
- Then choose Select Existing
- "Select Finish", and on the Publish page, select "Publish" to deploy the package containing your project files to your new function app in Azure
- After the deployment completes, the root URL of the function app in Azure is shown in the Publish tab
- From the left menu of the Function App window, select "Functions"
- Select "Get function url"
- The sum was calculated in Azure platform using the link that was gotten from "Get function url" in the function tab of azure function app that was created

