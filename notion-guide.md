
Notion document
[https://developers.notion.com/docs/create-a-notion-integration](https://developers.notion.com/docs/create-a-notion-integration)
# Step 1: Get notion secret token

A Notion integration lets you connect information in Notion to other software. To create your own integration:

1. Visit [https://www.notion.com/my-integrations](https://www.notion.com/my-integrations) in your browser.
2. Click the + New integration button.
3. Name the integration.
4. Select the [capabilities](https://developers.notion.com/docs/authorization#integration-capabilities) that your integration will have.
5. Click Submit to create the integration.

On the next page, you’ll find your Notion integration token, also called an API key. You’ll need this token to make requests to the Notion API. To retrieve your token after you leave this page, return to [https://www.notion.so/my-integrations](https://www.notion.so/my-integrations) and click View integration.
The integration has been added to the workspace, so any member can share pages and databases with it. There’s no requirement to be an Admin to share information with an integration.
### Creat new integration
![image.png](https://cdn.nlark.com/yuque/0/2023/png/703316/1678775435165-a5c1ef4e-d30b-416c-bcc0-492c9a2bc9bb.png#averageHue=%23fbfaf8&clientId=ua3cbe217-ad33-4&from=paste&height=629&id=u4396154a&name=image.png&originHeight=944&originWidth=1737&originalType=binary&ratio=1.5&rotation=0&showTitle=false&size=88374&status=done&style=none&taskId=ubc9d1c1c-58e1-4928-9717-01668ca2200&title=&width=1158)
### Fill information
![image.png](https://cdn.nlark.com/yuque/0/2023/png/703316/1678775643956-e6edd814-0434-4318-a8bf-8eb45669cd66.png#averageHue=%23fbfaf8&clientId=u4cd8df99-3888-4&from=paste&height=776&id=u68321623&name=image.png&originHeight=1164&originWidth=1390&originalType=binary&ratio=1.5&rotation=0&showTitle=false&size=125134&status=done&style=none&taskId=u8bdaca14-81ac-436b-86d8-e59e28ec5b8&title=&width=926.6666666666666)
![image.png](https://cdn.nlark.com/yuque/0/2023/png/703316/1678775666361-4d5d91b8-9917-441f-ad9f-10ba2e125ec1.png#averageHue=%23fcfbf9&clientId=u4cd8df99-3888-4&from=paste&height=794&id=u0fbc88a6&name=image.png&originHeight=1191&originWidth=1245&originalType=binary&ratio=1.5&rotation=0&showTitle=false&size=127803&status=done&style=none&taskId=u6c18b19b-b36d-4c18-b5d6-a3926c8892c&title=&width=830)

### Copy secret token
click the "Show" button ， and then copy the token.
![image.png](https://cdn.nlark.com/yuque/0/2023/png/703316/1678775749355-f10d79b0-5eae-4dcf-a1a7-5ec848d20b97.png#averageHue=%23f9f8f6&clientId=u92dd517b-8487-4&from=paste&height=503&id=u9e7f41d5&name=image.png&originHeight=754&originWidth=1293&originalType=binary&ratio=1.5&rotation=0&showTitle=false&size=97219&status=done&style=none&taskId=ua225fb5f-b136-4312-a06e-2d407fa94c7&title=&width=862)

# 
Step 2: Share a database with your integration
Now that you’ve created an integration, you need to grant it access to a database. To keep your information secure, integrations don't have access to any pages or databases in the workspace at first. **You must share specific pages with an integration in order for the API to access those pages**. To share a database with your integration:

1. Go to the database page in your workspace.
2. Click the **•••**on the top right corner of the page.
3. At the bottom of the pop-up, click Add connections.
4. Search for and select your integration in the Search for connections... menu.

Your integration now has permission to edit the database.
![image.png](https://cdn.nlark.com/yuque/0/2023/png/703316/1678776610779-05c11b30-567a-4eef-84b1-40ab47d4370a.png#averageHue=%23f9f9f9&clientId=u49209b4f-d7f3-4&from=paste&height=779&id=u0a517030&name=image.png&originHeight=1169&originWidth=799&originalType=binary&ratio=1.5&rotation=0&showTitle=false&size=121661&status=done&style=none&taskId=u8dc77daa-c6e9-4204-9668-6db8a0fe067&title=&width=532.6666666666666)
# Step 3: Get the database ID
You’ll need the database ID to edit the database using your Notion integration.
To get the database ID, copy the URL of your Notion database. If you're using an inline database, then make sure you're viewing the database as a full page. If you're using the Notion desktop app, then click Share and select Copy link to find the database URL.
The database ID is the string of characters in the database URL that is between the slash following your workspace name (if you named it) and the question mark. The ID is 32 characters long, containing numbers and letters.
![](https://cdn.nlark.com/yuque/0/2023/png/703316/1678775882567-b7f0111d-2ce0-4379-8eae-9c3975ca04d7.png#averageHue=%23dedbd7&clientId=u49209b4f-d7f3-4&from=paste&id=u771e55fe&originHeight=128&originWidth=1502&originalType=url&ratio=1.5&rotation=0&showTitle=false&status=done&style=none&taskId=u7ccfd437-09a1-450c-8fac-2e91d1d2fef&title=)
_Notion Database ID_
Copy the ID and paste it somewhere that you can easily find it for the next step.

![image.png](https://cdn.nlark.com/yuque/0/2023/png/703316/1678776307156-80239f8a-4bfa-4981-863d-a3e200174687.png#averageHue=%23fbfbfb&clientId=u49209b4f-d7f3-4&from=paste&height=609&id=u743aa38a&name=image.png&originHeight=914&originWidth=1666&originalType=binary&ratio=1.5&rotation=0&showTitle=false&size=87973&status=done&style=none&taskId=uc37975fd-9560-42d8-8268-b88130aafa0&title=&width=1110.6666666666667)
