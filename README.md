# AI In a box
Wrapper API layer on top of Azure/aws/GCP developer AI services. End user don't need to worry about back-end complexity, they need to call single API but switch between cloud

![Architecture](AI-In-Abox.png)

1) Platfrom-specific Components
These will host the service compnent needed to achive certail AI goal i.e. Text Translation, Document comprehension, etc 

2) AI Action Orcestration
Because each cloud has diffrent requirement like authentecation, files location etc. We need an orchestration layer which does the hard work so that end-use experience is simplified.

3) APIs/Actions Discovery
This wehre end-user discver and call all the back-end API. Business monitoring, Authentication, security will be done on that layer.

