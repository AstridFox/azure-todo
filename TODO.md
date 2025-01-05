# Building a Todo List App with Angular and Azure

## Development Setup
- **Angular**: Install Node.js and npm. Use npm to install Angular CLI globally.
- **Azure**: Set up an Azure account and install Azure CLI.

## Angular App Setup
- Use Angular CLI to create a new project: `ng new todo-app`.
- Structure the app with components for tasks and services for state management.

## Azure Functions
- Create an Azure Functions app in the Azure portal.
- Develop functions for CRUD operations, interfacing with CosmosDB.
- Test locally using Azure Functions Core Tools.

## CosmosDB Integration
- Set up a CosmosDB instance for storing tasks.
- Use Azure Cosmos DB SDK in Azure Functions for database operations.

## Azure Blob Storage for Static Files
- Configure Azure Blob Storage for hosting the Angular app.
- Set up Angular build to output files to a Blob Storage container.

## Connecting Angular with Azure Functions
- In Angular services, use `HTTPClient` for requests to Azure Functions.
- Ensure CORS settings are configured in Azure Functions.

## CI/CD with GitHub Actions
- **Repository Setup**: Initialize a GitHub repo and push your project code.
- **Workflow Configuration**: Create GitHub Actions workflows for building Angular and deploying with Azure Functions and Blob Storage.
- **Angular Build and Test**: Include steps in the workflow to install dependencies, build the project, and run tests.
- **Deploy to Azure Blob Storage**: Use Azure CLI in GitHub Actions to upload the Angular build to Blob Storage.
- **Deploy Azure Functions**: Utilize `Azure/functions-action` to deploy functions directly from the repository.

## Security and Monitoring
- Add authentication using Azure Active Directory.
- Use Azure Monitor and Application Insights for application monitoring.

## Theming with Angular Material
- **Installation**: Add Angular Material to your project and set up a custom theme using its theming capabilities.
- **Usage**: Utilize Material components throughout your Angular app to maintain consistent styling and behavior.
