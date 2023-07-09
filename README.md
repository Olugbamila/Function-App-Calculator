# Function-App-Calculator
 Pushing Application Into Azure Function App Through Visual Studio Code
## Create Function App  
- Login into visual studio code
## Create a New Project  
- Name your project
- Use http as trigger
## Apply Calculator Code
- Add sum to line 13
- Add sum to line 15
- int x =int.Parse(req.Query["x"]); line 22
- int y =int.Parse(req.Query["y"]) line 23
- int result = x + y line 24
- return new OkobjectResult(result); line 25
