# SharePoint list to QnAMaker using Microsoft Flow

## Deployment instructions
* Create list in SharePoint
* Download packages from GitHub repo
* Import packages to Microsoft flow and create new flow
* Fix SharePoint connection and change site URL and list
* Update the subscription id and KB id in the variables by editing the flow

## Things to be noted
* This flow will be adding questions to the prod version of QnAMaker KB.
* Its unidirectional, which means the changes will be always from SharePoint list and not the other way around, so any changes made directly in QnA Maker or through other direct APIs will not reflect on SharePoint list.
* Updating the question in SharePoint will add an alternate question in KB and it won't remove the previous question. Delete and newly add the question if required.
* Currently no other meta data is added to the question, add Github to your watch list for the future updates.
* Create an issue in the Github repo, I'll address if time permits
