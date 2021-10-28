# AI In a box
Wrapper API layer on top of Azure/aws/GCP developer AI services. End user don't need to worry about back-end complexity, they need to call single API but switch between cloud

![Architecture](AI-In-Abox.png)

1) Platfrom-specific Components
These will host the service compnent needed to achieve certain AI goal i.e. Text Translation, Document comprehension, etc 

2) AI Action Orcestration
Since each cloud provider has diffrent requirements like authentecation, files location etc. We need an orchestration layer which does the hard work so that end-use experience is simplified.

3) APIs/Actions Discovery
This wehre end-user discover and call all the back-end API. Business monitoring, Authentication, security will be done on that layer.

# Deployment steps:
1) Create a Translator Service in a resource group
2) Click: [![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsaffiali%2FAI-In-a-box%2Fmain%2Fdeploy%2FtranslationOrchestartor.template.json)
3) Pass the resource group name, sunbscription ID and Azure Translator API key to deployment parameters.

