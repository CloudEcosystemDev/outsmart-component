# <p align="center" width="100%"> <img src="./logo.png" maxwidth="350"> </p> 
# <p align="center" width="100%"> OpenApi OIH Connector </p>

## Description

A generated OIH connector for the OpenApi API (version 1.0).

Generated at: 2021-09-16T17:53:59+02:00

## API Description

FORMAT: 1A<br/>
HOST: https://www.out-smart.com/openapi/8<br/>
<br/>
# OutSmart<br/>
<br/>
OutSmart OPENApi<br/>
<br/>
## Changelog<br/>
<br/>
### API 8 <br/>
<br/>
+ 26-02-2020<br/>
	+ Added TimeSheet Hours, TimeSheet Travel, TimeSheet Expenses, Notes and Expense categories.<br/>
<br/>
+ 18-06-2019<br/>
    + Projects: added adr_code, cpn_code and debtor_number_invoice<br/>
+ 24-10-2018<br/>
    + Added section: Advanced filters<br/>
    + object_parts: Added advanced filters<br/>
+ 23-10-2018<br/>
    + Added endpoint: object_parts/changed<br/>
    + DeleteEntity: Added object_part entity<br/>
+ 17-10-2018<br/>
    + Deprecated endpoint: parts<br/>
    + object_parts: Added new fields<br/>
+ 07-08-2018<br/>
    + Added endpoint: invoices<br/>
    + Added endpoint: transactions<br/>
+ 21-06-2018<br/>
    + Added endpoint: vehicles<br/>
    + Added endpoint: regions<br/>
    + DeleteEntity: Added region entity<br/>
    + DeleteEntity: Added region entity<br/>
<br/>
+ 12-06-2018<br/>
    + PostWorkorders: Added Workperiods array   <br/>
    + PostWorkorders: Added 'MaterialType','MaterialFreeField1','MaterialFreeField2','MaterialFreeField3','MaterialFreeField4','MaterialFreeField5'<br/>
    + PostWorkorders: Added CustomerLatitude and CustomerLongitude<br/>
    + GetWorkorder(s): Added 'MaterialType','MaterialFreeField1','MaterialFreeField2','MaterialFreeField3','MaterialFreeField4','MaterialFreeField5'<br/>
    + GetWorkorder(s): Added CustomerLatitude and CustomerLongitude<br/>
    + addresses: Added adr_latitude and adr_longitude<br/>
    + relations: Added latitude and longitude<br/>
    + materials: Added eancode and barcode to docs<br/>
    + materials: Added freefield1, freefield2, freefield3, freefield4, freefield5 <br/>
    + Added endpoint: priorities<br/>
    + Added endpoint: errors<br/>
    + Added endpoint: solutions<br/>
    + Added endpoint: material_types <br/>
    + DeleteEntity: Added material_category entity<br/>
    + DeleteEntity: Added error entity<br/>
    + DeleteEntity: Added solution entity<br/>
    + DeleteEntity: Added priority entity<br/>
    + GetWorkorder(s): Added ShortWorkDescription,Comment,ErrorCode,ErrorMessage,SolutionCode,SolutionMessage,MinimumHours,RoundingAmount,PriorityCode,PriorityMessage<br/>
    + PostWorkorders: Added ShortWorkDescription,Comment,ErrorCode,ErrorMessage,SolutionCode,SolutionMessage,MinimumHours,RoundingAmount,PriorityCode,PriorityMessage<br/>
    + Changed Date and Time format in documentation to d-m-Y and H:i<br/>
    <br/>
+ 22-05-2018<br/>
    + objects: added parameter obj_adr_code, obj_latitude, obj_longitude<br/>
    <br/>
+ 28-02-2018<br/>
    + DeleteEntity: Added location entity<br/>
    + Locations: Added POST method<br/>
    + UpdateWorkorder: Added workstatus parameter<br/>
<br/>
+ 15-02-2018<br/>
    + objects: Added obj_order<br/>
    + objects/changed: Added obj_order<br/>
    + Added Endpoint: object<br/>
    + Added Endpoint: address<br/>
    + Added Endpoint: contactperson<br/>
    + Added Endpoint: category<br/>
    + DeleteEntity: Added object entity<br/>
    + DeleteEntity: Added address entity<br/>
    + DeleteEntity: Added contactperson entity<br/>
    + DeleteEntity: Added category entity<br/>
    <br/>
    <br/>
+ 18-12-2017<br/>
    + Added Endpoint: objects/changed<br/>
    <br/>
+ 22-11-2017<br/>
    + PostWorkorders: Added CpnCode and AdrCode<br/>
    + GetWorkorder(s): Added CpnCode and AdrCode<br/>
    + Added Endpoint: addressess<br/>
    + Added endpoint: contactpersons<br/>
+ 27-09-2017<br/>
    + PostWorkorders: Data and FileName to Attachments<br/>
    + GetWorkorder(s): Added PdfUrl to Forms<br/>
<br/>
<br/>
+ 06-04-2017<br/>
    + obj_object: Changed  `obj_debiteur_nummer` to required<br/>
+ 05-04-2017<br/>
    + GetWorkorders: Added `workstatus` parameter to GET parameters<br/>
+ 02-03-2017<br/>
    + Response object parameter `object` renamed to `response` due to reserved keywords in certain programming languages.<br/>
    + PostWorkorders: added WorkEndDate<br/>
    + PostWorkorders: added WorkEndTime<br/>
    + PostWorkorders: renamed WorkInstruction to WorkDescription<br/>
    + PostWorkorders: added InternalWorkDescription: This description is used to internally brief the employee. This field is not visible for the customer.<br/>
    + PostWorkorders: added WorkDeadline: This date can be added when no actual WorkDate and WorkTime are present. By setting the deadline the backoffice has the ability to prioritize unscheduled workorders<br/>
    + PostWorkorders: added WorkDuration: This value should contain the amount of scheduled minutes for the workorder. This is used for planning (setting WorkEndDate and WorkEndTime).<br/>
    + PostWorkorders: added WorkStatus: This status code can be selected from a list of work statusses (see new status API). The backoffice has the ability to add an extra status, for example: unable to contact customer, waiting for materials. When the employee completes the workorder and sets WorkFinished to 0  there is an option to select the reason, for example: bad weather conditions, customer not on location.<br/>
    + PostWorkorders: added PickupPlanning: Pickup planning will be used in the future to give the employees an option to pick their own workorders from a batch.<br/>
    + PostWorkorders: added WebPlanning: Web planning will be used in the future to give the customer an option to select their own WorkDate and WorkTime.<br/>
    + GetWorkorder(s): added WorkEndDate, WorkEndTime, InternalWorkDescription, WorkDeadline, WorkDuration, WorkStatus, PickupPlanning and WebPlanning<br/>
    + GetWorkorder(s): added Forms<br/>
    + GetWorkorder(s): added Archived to documentation<br/>
    + GetWorkorder(s): removed JobNr<br/>
    + GetWorkorder(s): renamed `photos` to `Photos`<br/>
    + GetWorkorder(s): renamed `workperiods` to `Workperiods`<br/>
    + GetWorkorder(s): renamed `materials` to `Materials`<br/>
    + GetWorkorder(s): renamed `documents` to `Documents`  <br/>
    + PostWorkorders: added Forms<br/>
    + PostWorkorders: added Employees: Relation between workorder and employees will be visible in planbord.<br/>
    + PostWorkorders: added WorkObjects<br/>
    + Added endpoint: forms<br/>
    + Added endpoint: suppliers<br/>
    + Added endpoint: objects<br/>
    + Added endpoint: parts<br/>
    + Added endpoint: object_parts<br/>
    + Added endpoint: categories<br/>
    + Added endpoint: material_categories<br/>
    + Added endpoint: worktypes<br/>
    + Added endpoint: paymentsmethods<br/>
    + Added endpoint: workstatusses<br/>
    + Response codes: added 1900, 1901, 2000, 2001, 2100, 2101, 2200, 2201, 2300, 2301, 2400, 2401, 2500, 2501, 2600, 2601, 2700, 2701, 2800, 2801 <br/>
    + relations: `email` changed to not required<br/>
    + added Workorder status section<br/>
    + added API workflow section<br/>
<br/>
+ 01-03-2017<br/>
    + Initial release<br/>
    <br/>
<br/>
## Authentication<br/>
<br/>
Each request should contain two GET parameters containing the customer and software token.<br/>
<br/>
+ Parameters<br/>
    + token<br/>
    + software_token  <br/>
<br/>
A token is registered to a WorkOrderApp customer who registered a license for an external software package. A software token is generated by WorkOrderApp and connected to a single external software package. When a request is executed we check if the external software packages connected to the token are matched.<br/>
<br/>
## Request<br/>
<br/>
Each request should be executed on the HTTPS endpoint. HTTP is not allowed and will result in an error. <br/>
<br/>
## Response<br/>
<br/>
Each request results in a JSON object with the following parameters:<br/>
  <br/>
- code: `1001` (number) - The response code of the executed request,<br/>
- messages:  (array[string]) - Array containing detailed messages of the executed request,<br/>
- response: (object) - Response object  <br/>
<br/>
Following code can occur in a response: <br/>
<br/>
| Code | Meaning                                                                                                                                   |<br/>
|------|-------------------------------------------------------------------------------------------------------------------------------------------|<br/>
| 200  | Request successfully executed.                                                                                                            |<br/>
| 1000 | The URL being called is not containing an endpoint.                                                                                       |<br/>
| 1001 | The endpoint being provided is unknown on our side.                                                                                       |<br/>
| 1002 | Request is missing the GET parameter: token.                                                                                              |<br/>
| 1003 | Request is missing the GET parameter: software_token.                                                                                     |<br/>
| 1004 | Client token provided is unauthorized to execute this request.                                                                            |<br/>
| 1005 | Software token provided is unauthorized to execute this request. Either the token is not correct or it's not matched to the client token. |<br/>
| 1006 | All endpoints should use https.                                                                                                           |<br/>
| 1007 | A general uncaught error occured. Please let WorkorderApp know.                                                                           |<br/>
| 1008 | The server did not receive a message body.                                                                                                |<br/>
| 1009 | The server did receive a message body but was unable to parse this to a valid JSON array or object.                                       |<br/>
| 1100 | The insert or update of an employee failed.                                                                                               |<br/>
| 1101 | A required field is missing in this request.                                                                                              |<br/>
| 1200 | The insert or update of a material row failed.                                                                                            |<br/>
| 1201 | A required field is missing in this request.                                                                                              |<br/>
| 1300 | The insert or update of a relation failed.                                                                                                |<br/>
| 1301 | A required field is missing in this request.                                                                                              |<br/>
| 1400 | No location data found for this customer.                                                                                                 |<br/>
| 1500 | Workorder not found by given criteria.                                                                                                    |<br/>
| 1501 | Posted workorder is missing a required field.                                                                                             |<br/>
| 1502 | Update workorder request is missing update data.                                                                                          |<br/>
| 1503 | No data changed.                                                                                                                          |<br/>
| 1504 | There was problem parsing the data being added.                                                                                           |<br/>
| 1600 | Delete of an entity failed.   <br/>
| 1700 | The insert or update of an project failed.                                                                                               |<br/>
| 1701 | A required field is missing or date is invalid in this request.                                                                                           |<br/>
| 1800 | The insert or update of a hourtype  failed.                                                                                                |<br/>
| 1801 | A required field is missing, active is not 1 or 0 or price cannot be parsed in this request.                                                                                              |<br/>
| 1900 | The insert or update of an object failed.                                                                                               |<br/>
| 1901 | A required field is missing.                                                                                              |<br/>
| 2000 | The insert or update of a supplier failed.                                                                                               |<br/>
| 2001 | A required field is missing.                                                                                              |<br/>
| 2100 | The insert or update of a part failed.                                                                                               |<br/>
| 2101 | A required field is missing.                                                                                              |<br/>
| 2200 | The insert or update of an object part failed.                                                                                               |<br/>
| 2201 | A required field is missing.                                                                                              |<br/>
| 2300 | The insert or update of a form failed.                                                                                               |<br/>
| 2301 | A required field is missing.                                                                                              |<br/>
| 2400 | The insert or update of a category failed.                                                                                               |<br/>
| 2401 | A required field is missing.                                                                                              |<br/>
| 2500 | The insert or update of a material category failed.                                                                                               |<br/>
| 2501 | A required field is missing.                                                                                              |<br/>
| 2600 | The insert or update of a worktype failed.                                                                                               |<br/>
| 2601 | A required field is missing                                                                                              |<br/>
| 2700 | The insert or update of a payment method failed.                                                                                               |<br/>
| 2701 | A required field is missing.                                                                                              |<br/>
| 2800 | The insert or update of a workstatus failed.                                                                                               |<br/>
| 2801 | A required field is missing.                                                                                              |<br/>
<br/>
### Example JSON<br/>
<br/>
+ Body<br/>
<br/>
        {<br/>
          "code": 1001,<br/>
          "messages": [],<br/>
          "response": null<br/>
        }<br/>
<br/>
## Workorder status<br/>
<br/>
A workorder status can be one of the following:<br/>
<br/>
| Status        | Description                                                                                           |<br/>
|---------------|-------------------------------------------------------------------------------------------------------|<br/>
| Klaargezet    | Workorder is created and ready to be fetched on a device (if an employee is selected) .               |<br/>
| Opgehaald     | Workorder is fetched on a device and employee can complete it.                                        | <br/>
| Compleet      | Workorder is completed and set to backoffice. Workorder is now ready to be administratively handled.  |<br/>
| Afgehandeld   | Workorder is administratively handled.                                                                | <br/>
<br/>
## API workflow<br/>
<br/>
+ Steps<br/>
    + Sync required entities to WorkorderApp<br/>
    + Add workorders through `PostWorkorders` API<br/>
    + Update workorders through `UpdateWorkorder` API<br/>
    + Fetch workorders through `GetWorkorders` with status Compleet. Add update_status=false to endpoint to prevent changing the status to Afgehandeld directly.<br/>
    + For each workorder with status Compleet process it.<br/>
    + If process is successfully completed call `GetWorkorder` API with update_status=true. The workorder status is now changed to Afgehandeld and will not be shown in next `GetWorkorders` call.<br/>
    + If an error occurs notify the user and act correspondingly.<br/>
<br/>
## Advanced filters<br/>
<br/>
<br/>
Filters can be given by adding a key and values array to the URL.<br/>
Adding a single filter: &key=key1&value=value1&operator=gt<br/>
Adding multiple filters: &key[]=key1&value[]=value1&operator[]=eq&key[]=key2&value[]=value2&operator[]=gt<br/>
<br/>
Following operators are allowed:<br/>
| Operator | Description                 |<br/>
|----------|-----------------------------|<br/>
| li       | Like (%)                    |<br/>
| eq       | Equal (=)                   |<br/>
| ne       | Not equal (!=)              |<br/>
| gt       | Greather than (>)           |<br/>
| ge       | Greather than or equal (>=) |<br/>
| lt       | Less than  (<)              |<br/>
| le       | Less than or equal (<=)     |<br/>
 <br/>
 <br/>
 <br/>
## employees [/employees/{?token,software_token}]<br/>
<br/>
This api is used to get or edit employees in WorkorderApp. <br/>
<br/>
Each employee record can contain the following data:<br/>
<br/>
| Parameter  | Required | Type (size)   |<br/>
|------------|----------|---------------|<br/>
| firstname  | Y        | Varchar (255) |<br/>
| lastname   | Y        | Varchar (255) |<br/>
| number     | Y        | Varchar (255) |<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add employees [POST]<br/>
<br/>
+ Request Correct employee data posted. `response` will contain the amount of employees synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
            [{"firstname":"Jan","lastname":"Klaassen","number":"123"},{"firstname":"Katrien","lastname":"Klaassen","number":"129"}]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": 2<br/>
            }<br/>
  <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"lastname":"Klaassen","number":"123"},{"firstname":"Katrien","lastname":"Klaassen","number":"129"}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1101,<br/>
              "messages": [<br/>
                "Required field missing: firstname"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
  <br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
            [{"firstname"":"Jan","lastname":"Klaassen","number":"123"},{"firstname":"Katrien","lastname":"Klaassen","number":"129"}]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1009,<br/>
              "messages": [<br/>
                "Unable to parse body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1008,<br/>
              "messages": [<br/>
                "Unable to fetch body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
### Get employees [GET]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [{"firstname":"Jan","lastname":"Klaassen","number":"123","active":"1"},{"firstname":"Katrien","lastname":"Klaassen","number":"129","active":"1"}]<br/>
            }<br/>
  <br/>
         <br/>
## materials [/materials/{?token,software_token}]<br/>
<br/>
This api is used to sync materials with WorkorderApp.<br/>
<br/>
Each material record can contain the following data:<br/>
<br/>
| Parameter    | Required | Type (size)   |<br/>
|--------------|----------|---------------|<br/>
| code         | Y        | Varchar (255) |<br/>
| description  | Y        | Text (64kb)   |<br/>
| price        | Y        | Decimal       |<br/>
| unit         | Y        | Varchar (255) |<br/>
| eancode      | N        | Varchar (55)  |<br/>
| barcode      | N        | Varchar (55)  |<br/>
| freefield1   | N        | Varchar (255) |<br/>
| freefield2   | N        | Varchar (255) |<br/>
| freefield3   | N        | Varchar (255) |<br/>
| freefield4   | N        | Varchar (255) |<br/>
| freefield5   | N        | Varchar (255) |<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add materials [POST]<br/>
<br/>
+ Request Correct material data posted. `response` will contain the amount of materials synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"code":"00001","description":"Omschrijving 1","price":"4,55","unit":"M2","eancode":"","barcode":"","freefield1":"","freefield2":"","freefield3":"","freefield4":"","freefield5":""},{"code":"00012","description":"Omschrijving 2","price":"2,50","unit":"M2"}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": 2<br/>
            }<br/>
  <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"description":"Omschrijving 1","price":"4,55","unit":"M2"},{"code":"00012","description":"Omschrijving 2","price":"2,50","unit":"M2"}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1201,<br/>
              "messages": [<br/>
                "Required field missing: code"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
  <br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
            [{"code"":"00001","description":"Omschrijving 1","price":"4,55","unit":"M2"},{"code":"00012","description":"Omschrijving 2","price":"2,50","unit":"M2"}]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1009,<br/>
              "messages": [<br/>
                "Unable to parse body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1008,<br/>
              "messages": [<br/>
                "Unable to fetch body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
            <br/>
### Get materials [GET]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response":  [{"code":"00001","description":"Omschrijving 1","price":"4,55","unit":"M2"},{"code":"00012","description":"Omschrijving 2","price":"2,50","unit":"M2"}]<br/>
            }<br/>
<br/>
       <br/>
## categories [/categories/{?token,software_token}]<br/>
<br/>
This api is used to categories with WorkorderApp.<br/>
<br/>
Each category record can contain the following data:<br/>
<br/>
| Parameter                 | Description                                   | Required | Type (size)   |<br/>
|---------------------------|-----------------------------------------------|----------|---------------|<br/>
| cat_code                  | Category code                                 | Y        | Varchar (255) |<br/>
| cat_cat_code              | Parent category code part                     | N        | Varchar (255) |<br/>
| cat_name                  | Category name                                 | Y        | Varchar (255) |<br/>
| cat_image                 | Url of the image. POST: An external url should be provided.  GET: You will receive a workorderapp url.     | N        | Varchar (255)      |<br/>
| cat_display               | Indication if the category should be displayed| Y        | Int (10)      |<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add categories [POST]<br/>
<br/>
<br/>
+ Request Correct categories data posted. `response` will contain the amount of categories synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [<br/>
                {<br/>
                  "cat_code": "001",<br/>
                  "cat_name": "Ijzerwaren",<br/>
                  "cat_display": "1",<br/>
                  "cat_cat_code": ""<br/>
                  "cat_image": ""<br/>
                },<br/>
                {<br/>
                  "cat_code": "001-002",<br/>
                  "cat_name": "Schroefjes",<br/>
                  "cat_display": "0",<br/>
                  "cat_cat_code": "001"<br/>
                  "cat_image": ""<br/>
                },<br/>
                {<br/>
                  "cat_code": "001-003",<br/>
                  "cat_name": "Boutjes",<br/>
                  "cat_display": "0",<br/>
                  "cat_cat_code": "001"<br/>
                  "cat_image": ""<br/>
                }<br/>
            ]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {"code":200,"messages":[],"response":3}<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
        <br/>
            [<br/>
                {<br/>
                  "cat_name": "Ijzerwaren",<br/>
                  "cat_display": "1",<br/>
                  "cat_cat_code": ""<br/>
                  "cat_image": ""<br/>
                },<br/>
                {<br/>
                  "cat_code": "001-002",<br/>
                  "cat_name": "Schroefjes",<br/>
                  "cat_display": "0",<br/>
                  "cat_cat_code": "001"<br/>
                  "cat_image": ""<br/>
                },<br/>
                {<br/>
                  "cat_code": "001-003",<br/>
                  "cat_name": "Boutjes",<br/>
                  "cat_display": "0",<br/>
                  "cat_cat_code": "001"<br/>
                  "cat_image": ""<br/>
                }<br/>
            ]<br/>
        <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 2401,<br/>
              "messages": [<br/>
                "Required field missing: cat_code"<br/>
              ],<br/>
              "response": null<br/>
            } <br/>
            <br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [<br/>
                {<br/>
                  "cat_code"": "001",<br/>
                  "cat_name": "Ijzerwaren",<br/>
                  "cat_display": "1",<br/>
                  "cat_cat_code": ""<br/>
                  "cat_image": ""<br/>
                }<br/>
            ]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1009,"messages":["Unable to parse body"],"response":null}<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1008,<br/>
              "messages": [<br/>
                "Unable to fetch body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
### Get categories [GET]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [<br/>
                {<br/>
                  "cat_code": "001",<br/>
                  "cat_name": "Ijzerwaren",<br/>
                  "cat_display": "1",<br/>
                  "cat_cat_code": ""<br/>
                },<br/>
                {<br/>
                  "cat_code": "001-002",<br/>
                  "cat_name": "Schroefjes",<br/>
                  "cat_display": "0",<br/>
                  "cat_cat_code": "001"<br/>
                },<br/>
                {<br/>
                  "cat_code": "001-003",<br/>
                  "cat_name": "Boutjes",<br/>
                  "cat_display": "0",<br/>
                  "cat_cat_code": "001"<br/>
                }<br/>
              ]<br/>
            }<br/>
<br/>
## category [/category/?token={token}&software_token={software_token}&key={key}&value={value}]<br/>
<br/>
This api is used to fetch category based on a filter. <br/>
Filters can be given by adding a key and values array to the URL.<br/>
Adding a single filter: &key=key1&value=value1<br/>
Adding multiple filters: &key[]=key1&value[]=value1&key[]=key2&value[]=value2<br/>
<br/>
### Get categories by filter [GET]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
               "response": [<br/>
                {<br/>
                  "cat_code": "001",<br/>
                  "cat_name": "Ijzerwaren",<br/>
                  "cat_display": "1",<br/>
                  "cat_cat_code": ""<br/>
                },<br/>
                {<br/>
                  "cat_code": "001-002",<br/>
                  "cat_name": "Schroefjes",<br/>
                  "cat_display": "0",<br/>
                  "cat_cat_code": "001"<br/>
                },<br/>
                {<br/>
                  "cat_code": "001-003",<br/>
                  "cat_name": "Boutjes",<br/>
                  "cat_display": "0",<br/>
                  "cat_cat_code": "001"<br/>
                }<br/>
              ]<br/>
            }<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
    + key (array,optional) ... Filter column, can be any of the allowed parameters.<br/>
    + value (array,optional) ... Filter value.<br/>
<br/>
   <br/>
## material_categories [/material_categories/{?token,software_token}]<br/>
<br/>
This api is used to sync material categories with WorkorderApp.<br/>
<br/>
Each material_categories record can contain the following data:<br/>
<br/>
| Parameter                 | Description                                   | Required | Type (size)   |<br/>
|---------------------------|-----------------------------------------------|----------|---------------|<br/>
| mct_mat_code              | Material code                                 | Y        | Varchar (255) |<br/>
| mct_cat_code              | Category code                                 | Y        | Varchar (255) |<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add material categories [POST]<br/>
<br/>
<br/>
+ Request Correct categories data posted. `response` will contain the amount of material categories synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [<br/>
                {<br/>
                  "mct_mat_code": "001",<br/>
                  "mct_cat_code": "7"<br/>
                },<br/>
                {<br/>
                  "mct_mat_code": "001",<br/>
                  "mct_cat_code": "8"<br/>
                }<br/>
            ]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {"code":200,"messages":[],"response":2}<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
        <br/>
            [<br/>
                {<br/>
                  "mct_mat_code": "001"<br/>
                },<br/>
                {<br/>
                  "mct_mat_code": "001",<br/>
                  "mct_cat_code": "8"<br/>
                }<br/>
            ]<br/>
        <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 2501,<br/>
              "messages": [<br/>
                "Required field missing: mct_cat_code"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
            <br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [<br/>
                {<br/>
                  "mct_mat_code"": "001",<br/>
                  "mct_cat_code": "7"<br/>
                },<br/>
                {<br/>
                  "mct_mat_code": "001",<br/>
                  "mct_cat_code": "8"<br/>
                }<br/>
            ]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1009,"messages":["Unable to parse body"],"response":null}<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1008,<br/>
              "messages": [<br/>
                "Unable to fetch body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
### Get material categories [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [<br/>
                {<br/>
                  "mct_mat_code": "001",<br/>
                  "mct_cat_code": "7"<br/>
                }<br/>
              ]<br/>
            }<br/>
<br/>
## relations [/relations/{?token,software_token}]<br/>
<br/>
This api is used to sync external contacts with WorkorderApp.<br/>
<br/>
Each relation record can contain the following data:<br/>
<br/>
| Parameter        | Required | Type (size)   |<br/>
|------------------|----------|---------------|<br/>
| name             | Y        | Varchar (255) |<br/>
| debtor_number    | Y        | Varchar (255) |<br/>
| contact          | N        | Varchar (255) |<br/>
| phone_number     | N        | Varchar (255) |<br/>
| email            | N        | Varchar (255) |<br/>
| email_workorder  | N        | Varchar (255) |<br/>
| street           | Y        | Varchar (255) |<br/>
| house_number     | N        | Varchar (255) |<br/>
| postal_code      | Y        | Varchar (255) |<br/>
| city             | Y        | Varchar (255) |<br/>
| remark           | N        | Text (64kb)   |<br/>
| latitude         | N        | Float (10,6)  |<br/>
| longitude        | N        | Float (10,6)  |<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add relations [POST]<br/>
<br/>
<br/>
+ Request Correct relation data posted. `response` will contain the amount of relations synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"name":"Naam B.V.","debtor_number":"14233Aaa","contact":"Dhr. Piet Klaassen","phone_number":"0761625345","email":"vb@example.nl","email_workorder":"vb@example.nl","street":"Beatrixlaan","house_number":"132","postal_code":"1234AB","city":"Utrecht","remark":"Let op met parkeren hier."},{"name":"Naam2 BV","debtor_number":"152346","contact":"Dhr. Example","phone_number":"0761654637","email":"vb@example2.nl","email_workorder":"vb@example2.nl","street":"Clauslaan","house_number":"54","postal_code":"1234AX","city":"Amsterdam","remark":"Let op met parkeren hier."}]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": 2<br/>
            }<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
<br/>
            [{"debtor_number":"14233Aaa","contact":"Dhr. Piet Klaassen","phone_number":"0761625345","email":"vb@example.nl","email_workorder":"vb@example.nl","street":"Beatrixlaan","house_number":"132","postal_code":"1234AB","city":"Utrecht","remark":"Let op met parkeren hier."},{"name":"Naam2 BV","debtor_number":"152346","contact":"Dhr. Example","phone_number":"0761654637","email":"vb@example2.nl","email_workorder":"vb@example2.nl","street":"Clauslaan","house_number":"54","postal_code":"1234AX","city":"Amsterdam","remark":"Let op met parkeren hier."}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1301,<br/>
              "messages": [<br/>
                "Required field missing: name"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
  <br/>
              <br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"name"":"Naam B.V.","debtor_number":"14233Aaa","contact":"Dhr. Piet Klaassen","phone_number":"0761625345","email":"vb@example.nl","email_workorder":"vb@example.nl","street":"Beatrixlaan","house_number":"132","postal_code":"1234AB","city":"Utrecht","remark":"Let op met parkeren hier."},{"name":"Naam2 BV","debtor_number":"152346","contact":"Dhr. Example","phone_number":"0761654637","email":"vb@example2.nl","email_workorder":"vb@example2.nl","street":"Clauslaan","house_number":"54","postal_code":"1234AX","city":"Amsterdam","remark":"Let op met parkeren hier."}]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1009,<br/>
              "messages": [<br/>
                "Unable to parse body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1008,<br/>
              "messages": [<br/>
                "Unable to fetch body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
### Get relations [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [{"name":"Naam B.V.","debtor_number":"14233Aaa","contact":"Dhr. Piet Klaassen","phone_number":"0761625345","email":"vb@example.nl","email_workorder":"vb@example.nl","street":"Beatrixlaan","house_number":"132","postal_code":"1234AB","city":"Utrecht","remark":"Let op met parkeren hier.","latitude":null,"longitude":null},{"name":"Naam2 BV","debtor_number":"152346","contact":"Dhr. Example","phone_number":"0761654637","email":"vb@example2.nl","email_workorder":"vb@example2.nl","street":"Clauslaan","house_number":"54","postal_code":"1234AX","city":"Amsterdam","remark":"Let op met parkeren hier.","latitude":null,"longitude":null}]<br/>
            }<br/>
           <br/>
## projects [/projects/{?token,software_token}]<br/>
<br/>
This api is used to sync external projects with WorkorderApp.<br/>
<br/>
Each project record can contain the following data:<br/>
<br/>
| Parameter        | Required | Type (size)     |<br/>
|------------------|----------|-----------------|<br/>
| code             | Y        | Varchar (255)   |<br/>
| code_ext         | N        | Varchar (255)   |<br/>
| debtor_number    | Y        | Varchar (255)   |<br/>
| adr_code         | N        | Varchar (255)   |<br/>
| cpn_code                    | N        | Varchar (255)   |<br/>
| debtor_number_invoice       | N        | Varchar (255)   |<br/>
| status           | Y        | Varchar (255)   |<br/>
| name             | Y        | Varchar (255)   |<br/>
| description      | N        | Text            |<br/>
| progress         | N        | Integer         |<br/>
| date_start       | Y        | Varchar (255)   |<br/>
| date_end         | N        | Varchar (255)   |<br/>
| active           | N        | Integer (1 or 0)|<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add projects [POST]<br/>
<br/>
<br/>
+ Request Correct projects data posted. `response` will contain the amount of projects synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"code":"N001","code_ext":"","debtor_number":"3","adr_code": "5","cpn_code": "","debtor_number_invoice": null,"status":"Nieuw","name":"Project op nacalculatiebasis","description":"Dit project zal op nacalculatiebasis worden gefactureerd. Tarief voor dit project is 100 eur per uur. Inkopen worden met een opslag van 10% doorgefactureerd.","progress":"0","date_start":"2013-10-01","date_end":null,"active":"1"},{"code":"P002","code_ext":"","debtor_number":"3","adr_code": "5","cpn_code": "","debtor_number_invoice": null,"status":"Nieuw","name":"Opdracht met voorschot","description":"Project is begroot op 100 uren en wordt tegen vaste prijs van 10.000 eur gefactureerd. 50% zal vooruit worden gefactureerd.","progress":"0","date_start":"2013-10-01","date_end":null,"active":"1"}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": 2<br/>
            }<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
<br/>
            [{"code":"N001","code_ext":"","debtor_number":"3","adr_code": "5","cpn_code": "","debtor_number_invoice": null,"status":"","name":"Project op nacalculatiebasis","description":"Dit project zal op nacalculatiebasis worden gefactureerd. Tarief voor dit project is 100 eur per uur. Inkopen worden met een opslag van 10% doorgefactureerd.","progress":"0","date_start":"2013-10-01","date_end":null,"active":"1"},{"code":"P002","code_ext":"","debtor_number":"3","adr_code": "5","cpn_code": "","debtor_number_invoice": null,"status":"Nieuw","name":"Opdracht met voorschot","description":"Project is begroot op 100 uren en wordt tegen vaste prijs van 10.000 eur gefactureerd. 50% zal vooruit worden gefactureerd.","progress":"0","date_start":"2013-10-01","date_end":null,"active":"1"}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1701,<br/>
              "messages": [<br/>
                "Required field missing: status"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
  <br/>
              <br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"code"":"N001","code_ext":"","debtor_number":"3","adr_code": "5","cpn_code": "","debtor_number_invoice": null,"status":"Nieuw","name":"Project op nacalculatiebasis","description":"Dit project zal op nacalculatiebasis worden gefactureerd. Tarief voor dit project is 100 eur per uur. Inkopen worden met een opslag van 10% doorgefactureerd.","progress":"0","date_start":"2013-10-01","date_end":null,"active":"1"},{"code":"P002","code_ext":"","debtor_number":"3","adr_code": "5","cpn_code": "","debtor_number_invoice": null,"status":"Nieuw","name":"Opdracht met voorschot","description":"Project is begroot op 100 uren en wordt tegen vaste prijs van 10.000 eur gefactureerd. 50% zal vooruit worden gefactureerd.","progress":"0","date_start":"2013-10-01","date_end":null,"active":"1"}]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1009,<br/>
              "messages": [<br/>
                "Unable to parse body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1008,<br/>
              "messages": [<br/>
                "Unable to fetch body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
### Get projects [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [{"code":"N001","code_ext":"","debtor_number":"3","adr_code": "5","cpn_code": "","debtor_number_invoice": null,"status":"Nieuw","name":"Project op nacalculatiebasis","description":"Dit project zal op nacalculatiebasis worden gefactureerd. Tarief voor dit project is 100 eur per uur. Inkopen worden met een opslag van 10% doorgefactureerd.","progress":"0","date_start":"2013-10-01","date_end":null,"active":"1"},{"code":"P002","code_ext":"","debtor_number":"3","adr_code": "5","cpn_code": "","debtor_number_invoice": null,"status":"Nieuw","name":"Opdracht met voorschot","description":"Project is begroot op 100 uren en wordt tegen vaste prijs van 10.000 eur gefactureerd. 50% zal vooruit worden gefactureerd.","progress":"0","date_start":"2013-10-01","date_end":null,"active":"1"}]<br/>
            }<br/>
<br/>
## hourtypes [/hourtypes/{?token,software_token}]<br/>
<br/>
This api is used to sync external hourtypes with WorkorderApp.<br/>
<br/>
Each hourtype record can contain the following data:<br/>
<br/>
| Parameter        | Required | Type (size)         |<br/>
|------------------|----------|---------------------|<br/>
| code             | Y        | Varchar (255)       |<br/>
| name             | Y        | Varchar (255)       |<br/>
| cost_booking     | Y        | Integer (1 or 0)    |<br/>
| sale_booking     | Y        | Integer (1 or 0)    |<br/>
| sale_price       | Y        | Decimal (> 0)       |<br/>
| cost_price       | N        | Decimal (> 0)       | <br/>
| active           | N        | Integer (1 or 0)    |<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add hourtypes [POST]<br/>
<br/>
<br/>
+ Request Correct hourtypes data posted. `response` will contain the amount of hourtypes synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"code":"001","name":"Normale uren","cost_booking":"0","sale_booking":"0","sale_price":"50.00","cost_price":"25.00","active":"1"},{"code":"ZK","name":"Ziekte","cost_booking":"1","sale_booking":"1","sale_price":"0.00","cost_price":"0.00","active":"1"}]            <br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": 2<br/>
            }<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
<br/>
            [{"name":"Normale uren","cost_booking":"0","sale_booking":"0","sale_price":"50.00","cost_price":"25.00","active":"1"},{"code":"ZK","name":"Ziekte","cost_booking":"1","sale_booking":"1","sale_price":"0.00","cost_price":"0.00","active":"1"}]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1801,<br/>
              "messages": [<br/>
                "Required field missing: code"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
  <br/>
              <br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"code"":"001","name":"Normale uren","cost_booking":"0","sale_booking":"0","sale_price":"50.00","cost_price":"25.00","active":"1"},{"code":"ZK","name":"Ziekte","cost_booking":"1","sale_booking":"1","sale_price":"0.00","cost_price":"0.00","active":"1"}]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1009,<br/>
              "messages": [<br/>
                "Unable to parse body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1008,<br/>
              "messages": [<br/>
                "Unable to fetch body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
### Get hourtypes [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [{"code":"001","name":"Normale uren","cost_booking":"0","sale_booking":"0","sale_price":"50.00","cost_price":"25.00","active":"1"},{"code":"ZK","name":"Ziekte","cost_booking":"1","sale_booking":"1","sale_price":"0.00","cost_price":"0.00","active":"1"}]<br/>
            }<br/>
         <br/>
## forms [/forms/{?token,software_token}]<br/>
<br/>
This api is used to sync external forms with WorkorderApp.<br/>
<br/>
Each form record can contain the following data:<br/>
<br/>
| Parameter                 | Description                                                                                                               | Required | Type (size)   |<br/>
|---------------------------|---------------------------------------------------------------------------------------------------------------------------|----------|---------------|<br/>
| name                      | Name of the form                                                           | Y        | Varchar (255) |<br/>
| data                      | JSON data of the form                                                                 | N        | Text (64kb) |<br/>
| template                  | HTML template to display data in PDF                                                                   | N        | Text (64kb) |<br/>
<br/>
The `data` parameters contains a JSON encoded representation of the form. The main element is called `fields` and contains an array of JSON objects representing a `field`.<br/>
Each field contains the following data:<br/>
<br/>
| Parameter     | Description                                               |<br/>
|---------------|-----------------------------------------------------------| <br/>
| label         | The label of the field.                                   |  <br/>
| field_type    | The Type of the field. Can be `text`, `checkboxes`, `radio` , `dropdown` or `signature`.<br/>
| required      | This field indicates if the field is required to complete. Text: Field is valid a value is filled. Checkboxes: Field is valid when all the boxes are checked. Radio: Field is valid when a option is checked. Dropdown: Field is valid when a option is selected. Signature: Field is valid when a signature is set |<br/>
| cid           | Unique indentification of the field.                      |<br/>
| field_options | Array containing field options. See description below.    | <br/>
<br/>
<br/>
Each field_options contains the following data:<br/>
<br/>
| Parameter     | Description                                                                                   |<br/>
|---------------|-----------------------------------------------------------------------------------------------| <br/>
| options       | The options of the field. Used in `checkboxes`, `radio` , `dropdown`. See decription below    | <br/>
| value         | Value added in `text` field or base64 encoded image in `signature` field.                     |      <br/>
<br/>
 <br/>
Each options contains the following data:<br/>
<br/>
| Parameter     | Description                                                                       |<br/>
|---------------|-----------------------------------------------------------------------------------| <br/>
| checked       | Indicated if options is selected. Used in `checkboxes`, `radio` , `dropdown`.     | <br/>
| label         | Label for the option                                                              |      <br/>
<br/>
+ Sample JSON<br/>
    + Text:` {<br/>
      "label": "Serienummer",<br/>
      "field_type": "text",<br/>
      "required": true,<br/>
      "field_options": {<br/>
        "size": "small",<br/>
        "value": ""<br/>
      },<br/>
      "cid": "c6"<br/>
    }` <br/>
    + Radio: ` {<br/>
      "label": "Type pomp",<br/>
      "field_type": "radio",<br/>
      "required": true,<br/>
      "field_options": {<br/>
        "options": [<br/>
          {<br/>
            "label": "type A",<br/>
            "checked": false<br/>
          },<br/>
          {<br/>
            "label": "type B",<br/>
            "checked": false<br/>
          },<br/>
          {<br/>
            "label": "type C",<br/>
            "checked": false<br/>
          }<br/>
        ]<br/>
      },<br/>
      "cid": "c2"<br/>
    }`<br/>
    + Checkboxes: ` {<br/>
      "label": "Type pomp",<br/>
      "field_type": "checkboxes",<br/>
      "required": true,<br/>
      "field_options": {<br/>
        "options": [<br/>
          {<br/>
            "label": "type A",<br/>
            "checked": false<br/>
          },<br/>
          {<br/>
            "label": "type B",<br/>
            "checked": false<br/>
          },<br/>
          {<br/>
            "label": "type C",<br/>
            "checked": false<br/>
          }<br/>
        ]<br/>
      },<br/>
      "cid": "c2"<br/>
    }`<br/>
    + Dropdown: ` {<br/>
      "label": "Dropdown",<br/>
      "field_type": "dropdown",<br/>
      "required": true,<br/>
      "field_options": {<br/>
        "options": [<br/>
          {<br/>
            "label": "A",<br/>
            "checked": false<br/>
          },<br/>
          {<br/>
            "label": "B",<br/>
            "checked": false<br/>
          }<br/>
        ],<br/>
        "include_blank_option": false<br/>
      },<br/>
      "cid": "c10"<br/>
    }`<br/>
    + Signature: `{<br/>
      "cid": "c5",<br/>
      "field_options": {<br/>
        "value": "iVBORw0KGgoAAAANSUhEUgAAA6IAAAJYCAYAAAB4hltMAAAABHNCSVQICAgIfAhkiAAAIABJREFU\neJzt3V2wZlWZH/BnpvJ1l3Obm7x9k6tUd5HbabpirtJ2eTFV0sGrKBY1F4SuYEUlVFmiFJmhqi2d\nUYpBJzo4zhgUnR4UCOooRAERFVAIigLyIR+CNP1Bd9Mf57y5OP1mjmfOx7P2Xnvt9/T5/apWTc3M\n2ev5r5erp9fea0UAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nADCWHWMHAAAA4MJ3UUTcExHTFePaURMBERHxe2MHAABgS7ooIv79+f95USzvOD4aEfee/5+3jxXs\nvIsi4pF1/n/3RsR/aBcFAACAvj4Sv7vLuNZ4JJabwbEcXifXbLxntGQAAACkzXYZN2tCx34V9ppE\nrltGyAUAAECBhYh4Icqa0Nm4qnHWM4lM9zbOBAAAQKGvRLcmdBoRb0S7U2s/nsz0kUZ5AAAA6OAP\no3sTOhv3NMi5EBFLyTxjfr8KAADAJn4R/RvRaQy/K7r6qpb1xmMD5wA28U/GDgAAQMr+iPi3EfEH\nEfEvI+JcRPw2In4SEd+MiPsGqrsQEf+m0lwXRcSzleZabVdEvC35t+8YKAMAAMCW96mIeDNyu3yL\nEXFXLDeONR1M1h/7u8zHkxnuGDADAADAlvW96N7sLUXEgYpZjvbIsnrcWzHXSnuS9RejfqMOAACw\npV0b+cN2Nhufq5SpVhM6jYibK2Va7XCy/q0D1QcAANhyJhHxXNRt+qax/FptHwcq53lfzzxr2Z+s\nfW6A2gAAAFtS7WZv9djZI9uvKmcZ4sqUU8na1w9QGwAAYMt5KIZtQqcR8UqPfLVeE57G8veZtV2X\nrP3WALUBAAC2lD2x3BwN3YTOxp4OGRcqZ3iyQ4bNLCZrXzpAbQAAgC3j7mjXgM7G8x1yfqVyhtrN\n4BeTdY9XrgsAALBlXBoRJ6J9EzobpdeW1Ly2ZVpYezMlu7X7KtcGAADYEr4Z/Zq4MxHx9fiHZvKS\nWL6KpGSOTxRmrtmEHi6svZkHknX7fB8LAACwJe2KiJPRvYE7FxF7N5j/hoK5ThVmr9mIXldYeyOT\ngrp9TgwGAADYcm6Mfs3bt5J1SuacJOcsafYyo/S14I28kKz5aMWaAAAAc++l6N60nY6IiwtqZU+O\nncbyAUQZX++Rf/U4U7CWzewqqFuz+QUAAJhbk1h+nbZr03Zfh5olhwplT5B9tscaVo9bO6xpPceT\nNR+qWBMAAGBuvT26N2tvRffTXR8srJXxZo+1DLUzeVlBTQAAgAve/ujeqN3fs/YthfUOJOY802M9\nK0fN13JPJ2t+tmJNAACAuXRFdGvSzsVyA9vXvsK6P03MWfLd6UbjMxXWFxFxMFlvsVI9AACAudV1\nJ/TpyjlKap9OzLdUOOd6o5Zsnqsr1gQAAJg7Xb8JvWGALK8XZtjsu80ajejPKq3trmS9mq8BAwAA\nzJ3dUd6sLZ1/bgh3FmY5uMl8NRrRSYV1LRTUu7JCPQAAgLk0ifJG7WQMe69l6XeiL24yX99G9DeV\n1vVUsl72WhoAAIAtZyHK7wl9rVG2kkybHerT97CiGk33pKDeUDvNAAAAo1qI8mtNnt9kzndFxEMR\ncTiWv/P8zvn/WxfHCrNt9Opsn+tbvt0x/2q/TtZ7pVI9AACAubIQy6/XljRkz2wy37MbPPvdDhm/\nWJjvyxvMdbZwrtlY6pB7LbsLam7UUAMAAGxJCxFxIuo1oRHL3zRuNscPC3PuKsx4ZIO5un4j+geF\nmdeTbfqfrFQPAABgbnRpQn+1yZy/KJjr8sK8pQ3kWkpOql057ivMup4rCmoOeQAUAABAc12a0Jc2\nmfPThfM9XZi5xn2inymcYxoRpwpzbiT7WvBdFWsCAACMbhLlB/b8epM5byucbxoRpwtzlzaRn19j\njtOFcyxFxM7CnOu5oaAuAADABaNLE7rZzuVXCuebjc2uWVmt9LXa1VfL7OiQcX9hxo1kXy2+uWJN\nAACAUU2i/A7NzZrQPyqcb+U43mENJd+Jrm50HynM97kO+dbzjY6ZAQAAtqxdUX7Yz2anti5ExLnC\nOVeOv++wjsOFNVYqWf/PO2TbSLbuByrXBQAAGEWXJvSniXn/vnDOjZrErK92rHF5wTO1dyWfSNY9\nWbkuAADAKN4e5Q3iE4l5u16DMhvf6rie0rqzHcY3Cp65s2O2tUwK6r6zYl0AAIBRdGlCNzsdd+b7\nHeZeOS7tsa6SOl+KsmZwGhEX9ci22kvJmscq1gQAABjFO6O8OXwxOXff3dBpz7WVnPr7vYj4esHf\n12wIdxfUnVSsCwAA0NzeGK4JjYh4vMP8K8frfRYXy7u22VrPRdmBSn/VM9tKx5I1X6hYEwAAoLmS\nXbgujdCkw/yrx1d6rC8i4paCWkcKs+3omW2m5B8DFirVBAAAaG5nlDeF2W9CZ37aoUbtxmtXQa2S\n3dATPXOtdDZZ896KNQEAAJqaRPkVLaVNaBTOv9Z4rMviBsix1ri1UrZrC2oCAABsWYtR1nSVfBM6\n80BhjSF2Q2eGaERrZcv+t6jV+AIAADR3OIZvQqOwxlrjgY5111K6+7vZqPVa7heS9RYr1QMAAGiu\n9JvNVzrW+dvCOkPuOEaUXeGSGR+vlCtb78pK9QAAAJq6McqarcM9avXdgXy4R+21vN4zz+qxo0Km\nh5K1TleoBQAA0Ny+KGu03uxR64rCWkPvhkYsXzlTqwk9WiHPQkG9/RXqAQAANDWJssOJ+u7AvVVQ\na63x85711/J4z0wrx59XyPN0staxCrUAAACaOxr5Jmsx+u1G7iio1Wo3NCLizgq5auXbXVBrV89a\nAAAAzX07ypqsSc96Py6st3o83bP+eg71zDUbNV7LfTVZ69kKtQAAAJq6PsqarL0VavY9pGiI3dCI\n5ddpazSifV/LfXtBrb7/KAAAANDUrihrsK6uULOkyVpr/KpChvVc1TPbbPR1IlnnexVqAQAANPVm\n5Jur+yrVfKWgZsvd0Ig6jWjfg4Pem6yz1LMOAABAcz+KfHP1WsW6fZq8H1fMsZZ39Mw3jf6v5Z5N\n1vlszzoAAABNXRP5xupsxbr7C+quNYZ2ac98fTMeTNZY7FkHAACgqdLvQmteDfLrwtorx9cq5ljP\ngR75ptH/tdzsPa4HetYBAABoZiEi3op8Y3VN5fpdG7xW30N+qEfGaUR8skftv0nWONWjBgAAQHPP\nRr6pqnU40Uyf13LfWTnLej7fI+O0Z+1sjX096wAAADRzc+SbncMD1H++oP7K8fIAWdZza8eM04g4\n0qPud5M1Wv4WAAAAvZTsRi5FxGSADF2au9ZXlHy7Y85pRFzXseakoEbN73UBAAAGsxAR5yLf7Fw6\nQIZ3FdRfOd49QJaNPNgx57RHzZ8n53+sRw0AAICmXop8M3XbQBleLcgwG78cKMtGsk3h6tH1tdyS\nE4wXOtYAAABo6i8j3+i8PmCO0sbuzIBZNtKlYZ5GxJUd62X/keDOjvMDAAA0Vfpd6FA7btmDeFaO\nnQNl2cyRgowrRxfZ15UXw24oAACwBZR+F/reAXOUNnXvHyhLxqkNcq03up4wnG16b+w4PwAAQFPP\nRr6Run3AHN8ryDGNiPsHzJJxNsryTmN557nUgeTcp7svBQAAoJ2/iHwT9dqAOUp3Q/vcw1lLq9dy\n30rOfXnH+QEAAJrZHfkGaqj7QmeeK8iyOHCWjC6vET/boc4NybmPdl4JAABAQyXfhV42YI6Sa0mm\n5/9+bDdFeSO6u0OdpeTc+7ovBQAAoI2nI99A3TtwlpJrUK4ZOEtW6fehSx1qfC059/M91gEAANDE\n+yPfQL05cJaS14N/MnCWrEujfDf04cIaC5HfDXVdCwAAMNd2RlkDNRk4T/YgnnlquEp2k2djR2GN\n+5Lzjn1yMAAAwKZORL55OjhwlpLd0JsHzpLV5ZCi0mtVst/MLsX8NOcAAABrOhT55qnFd4fZ7yy7\nfF85lNujvBH9YmGNJ5Lzfr3fUgAAAIZV8kruYoM87y7IM0/3Yy5GeSNasmu5JznnPDXnAAAAaypp\noC6ZozxnGmTJem+UN6Gl93tmTxD+UL+lAAAADOtnkW+c7mqQ50MFefY0yJP1RpQ3ovsL5s+exnu8\n/1IAAACGszfyTVOr3cfstSRvNMqTMYnyJrT09dlTyXnf128pAAAAw8o2fdNY/o50aH9ckGfSIE/W\ng1HeiL5YMH/2d3mt/1IAAACG88vIN02fbJQpm+fZRnmyShr62Xhncu6FyH8ze2mV1QAAAAzg3ZFv\nmI41yvTZgkzz5Ioob0JL1pC9Vuen/ZcCAAAwnJJTclu9ApvNc3+jPFnZbze7NKILBfPtqrIaAACA\nAZSckvvpRpm+X5BpnuyKbk1odh3Zb09/WGU1AAAAA7gk8o1Sq4NvJgWZPtcoU9bT0a0JzZyYW9Lk\nttq1BgAAKFZyqE4rLyTzlF530kLX3dDTibmfS851d7XVAAAAVPZo5BulDzfKVHKP6Z80ypR1Q3Rv\nRA9vMve+5DyLNRcEAABQ0+7IN0m/aZjraDLTPO6Gno3ujehTm8x9PDnPTTUXBAAAUFNJ09TKewoy\nzdtuaJ9DiqYR8aUN5n5fco6zldcEAABQze2Rb5BuaJjrXDLTPL5++nr0a0Sv22Du7D8aXF15TQAA\nAFXsjHxzdLRhri8V5Jq3hqvkbs/1xmSduW9MPn+i/rIAAADqOBn9m6PaShq5eXz99M7o34iuZSHy\npxq/q/6yAAAA+vtC5BujTzbMVXL35jUNc2WVXIFT0oj+n+Szrw6wJgAAgN4mkW+KjjTMVXJ671sN\nc2UdiP5N6Lk15i3577VrkJUBAAD09GbkG5tJw1xHCnK9r2GurOx1MxuN19aY95nks08MsywAAIB+\nbop8U/RnDXPtLch1umGurL5XtszGnavmLdklthsKAADMnZJXPN9onG2xINtVjbNl/DTqNKJXrpo3\nexXMdwdbGQAAQA8lr45OGuY6VJDrVMNcJWo0odNVc15W8NzCYCsDAADo6GDkm5rPNs5W0qj9ceNs\nGbfEMI3omeQzh4ZaGAAAQFeTyDdChxtne64g21LjbFlno04TuvJe1Ow/HCwOujIAAICO3oh8MzRp\nmGtnQa5pRPxJw2xZe6LebugLK+bN3kd6cMjFAQAAdHFd5BuhTzXOVnKNzLmYz+8gX416jeinz895\nV/Lv5/V7WQAAYBtbiHwT1PqV3A8UZJtGxNca58vYEfWa0NludMl/s8sGXyEAAECh7NUfsyaopeyr\np9OY329D74m6jWhExBPJvz0y9OIAAABK3Rz5Bqj1d4bfKsg2jfk8FXYhyprpzcZiROwq+Ptdwy8R\nAAAg7+LINzQvrDPHUCYF2WZjHr8N/VDU3Q19NiJeS/7tS8MvDwAAoEz2ldylaP9KbrbZmo0HG+fL\nOhF1G9HsAUXTaP/fDAAAYEOfiXxDc3njbHsLss3zbug7om4TOo2I08m/e7jB+gAAANJKvjF8bIR8\niwX5phHx5AgZM34a9RvRrdyYAwAA21j2ddFz0f71zluT2ea96Sq5XqX2mMdDmwAAgG3sjsg3NFc1\nztaleWt9iFLWd2KcJnRer7ABAAC2qX2Rb2jGOPzn1YJ8szGv15PUvLKlZFzbYnEAAABZZyPXzJyM\n9q+7XpLMtnK82jhj1sdinCb0bIvFAQAAZD0W+YZmzwj5zhXkm429I+TMOBXjNKLz+nsAAADb0OWR\nb2buHiHfoYJ8s3FshJwZB2KcJvR4i8UBAABkTCJ/HcrJkfJ1abz2j5A1440YpxHd3WJxAAAAGS9F\nvpnZN0K+FwvyzcapEXJm7IlxmtBft1gcAABAxqci38z81Qj5LivIt3JcNkLWjKdinEZ0Hu9RBQAA\ntqFJ5BuZN0fKmH1leOU4M0rSzXW5A7XG+FGLxQEAAGSUnNw6xl2c9xTkWzmuHSFrxjej23pOdHxu\nNgAAAObC3ZFvZG4cIV/Jbu3KsThC1qyujeRbPZ491GRlAAAAm3hP5BuZw+NEjKMFGVeOz4wRNuGz\n0W09xzs+N+9NOQAAsM2UfHc5GSHf1QX5Vo6lEbJmnY1ua/rrjs9NI+KGJisDAADYxC8j38hcN0K+\nhVhuKLs0XneMkDej68m/04j4847PnWuyMgAAgE0cjHwjM9a9kz8qyLh6zKuT0W09D0bEEx2f3dtk\nZQAAABuYRL6JWYpx7p3cV5Bx9XhshLwZu6L7mnZExOkOz4111Q4AAMDveDPyjcxlI2Xsc03JGI1z\nxmvRbT1Hzz/f5dndwy8LAABgY4ci38T8ZAtkXD1eHCFvxkJ0X9MHI+IdHZ57vsnKAAAANrA78k3M\nWAfcTKL7AUXTGOdk34znovuaIiK+2uG5ef0tAACAbaSkwRvrgJuXCjKuHkfXmG8e9NkN/db5OV4p\nfO6R4ZcFAACwsWci38TcPVLGAwUZ56l53sx90X1Ns+9dzxU+BwAAMKr3R76BOT1SxoUob7ZWjlPt\nI6d1XdOR88/vKHzuM8MvCQAAYGMlTcxkpIz3F2Rca1zbPnLKF6P7mmYn3l5f8MxigzUBAABs6Ejk\nm5ibR8rY587QeW++uh68tHJNjxQ8N68NOQAAsE38WeQbmDdGyhgRcXyDXJnx5faRU66N7mv6ixXz\nLCafOTv0ggAAADayM8oan7F8cpNc85x9M2ej/5omBc/M62FNAADANnEs8g3MB0bKOIl+d4ZOI+Lh\n5qlz9kf3NT2xYp7fJJ85PPSCAAAANnJL5Jue58aJGBERz2+QKzsW/tGs86HP68a7zs9Rsqu9s8Ga\nAAAA1lTyKueYh/z0vTN0GhG/ap46p+S/wepxcsU82d3Qo0MvCAAAYCOnIt/0vHOkjAuRP4Bno3Fx\n6+BJz0b3Ne0/P8eeDs8AAAA094XINy8PjZQxIuKHG+TKjmPNU+csRPc1rTz1tuQfFAAAAEZR8jro\nmNd8XLpBrpJxoHXwpG9G9zVde36OkteW32ywJgAAgDWVnJI75sE2JzfItRUa6c10XdPSijlOFzz3\n/aEXBAAAsJaDkW9c7hopY0TEoQ1ylYyPtw6eVPLfYfX45vk5ri98bt/wywIAAPhdk8g3LWdGyhix\nfCVJjSZ0Keb3ypaz0X1dM6WHOAEAADRXchfnZKSMEcvfMtZoRO9vHTzpsui+psfPz/HFwud8HwoA\nADRXcqjNl0fKGBHx2Q1ylY4dbaOnvR7d17QQ3U7b/VqTlQEAAJxXchfn6ZEyRpS9OrzZeL5x9qwd\n0X1Nvz0/x3c7PLtr6IUBAACs9OPINyyTkTJG9NspXD32NM6e9WR0X9Mkuu2GrjxlFwAAYHAld3GO\n+UruRzfIVTqONc6e1aWJXL2mn3Z49teDrwwAAGCF7D2TF8orudOIuKpt/LTPR/c17Yrujez+FosD\nAACIWL4HNNus7B0pY0TELzbIVTrGvHZmM0vRbU2nzj9fcurxygEAANBEyV2c3xwpY0TZab6ZMa+n\nw/7X6L6myyJiX8dnX2qxOAAAgIjlE1YzjcrZsQKel90lzJ76O68OR7dGcvbK9Ksdn/daLgAA0MTB\nyDcq+0bKGBHx1Aa5uowfto2fVrI7vXp8MMoOnFo5nJYLAAA0UXJn6CMjZYyIuHKDXKvHK8m/u6jp\nCvIejW6N5Lnzz5/q+PwDg68MAAAg8td7LI4V8Lxss3w6cq/v/rZt/LSF6H5I0cGIuKbjs9PztQEA\nAAZV8grngZEyRkT8aoNcq8fXk3/3R01XkHdrdGsiZ/9QcKbj88cHXxkAAEDkX+H8xVgBo+yV3Acj\n14iNfeDSRs5Gt0byxoi4vuOz01g+aRcAAGBQd8fWeGUz+5rquchf7XJz0xXkvS+6NZGzQ4ayry+v\nt5sKAAAwmJJTWa8bKWNExHMb5Fo99kfEG8m/nddvIY9Ft0by1oj4QsdnpxFxW4vFAQAA29vxyDUo\nYx7o84ENcq0eT0a+uX685SIK7Inuu6GT6H7A0bTF4gAAgO3t5sg3KBePlDEi31jNXkvN3jG6q9kK\nyvwquu+Gfq3js7MmHgAAYDCTyDcoXxwpY0TEyxvkWj3eH8uv2mb+9nDLRRTI5l9vN7RrEzqN+X1N\nGQAAuEA8H7nm5NRYASPigxvkWj1eOP/MN5J//95Wiyj0QHRrIr8TES92fHYaEa+2WBwAALB9XR75\nBmXPSBljk1yrdwNnMqfFzuvJsAvR/fvOpzs+Nxv7G6wPAADYphYif7XHD0fKGLH86my2ibry/DPX\nJP/+q60WUeim6NZEZu+AXW+cbrE4AABg+/p+5JqTxVj+5nAMtyTyzcbLK547nXxmXp2Nfg1l13FN\ni8UBAADb077INycfGinjpCDjyqZyd/Lvn26xiA4OxDhN6LkWiwMAALavM5FrTsY8uKbkNdN3rnju\nt8ln5vXKljdjnEb0L1ssDgAA2J7uiXxzMlazdqgg4zMrnpsknzneYhEd7IpxmtBpuLIFAAAYSPa1\n1WlE/K+RMu4syLi06tkHk88dGHoRHb0S4zShYx5GBQAAXOCyr32eHStg5E/ynUbE3lXPZq48mecr\nW8baDZ3X15QBAIAt7sbINyb7Rsr4s4KM96969pPJ5+4aehEdfS/GaUJfbLE4AABg+5lEvjH55UgZ\nryzIuNaObfYApnmV2c0dYlzaYnEAAMD285vINSVLMd6hNSXN085Vz2a/fR3zFOCNfCbGaUJPtVgc\nAACw/Vwd+cbkupEylhzS8+k1ns9e2bJ7yEX0cDbGaUQ/3mJxAADA9pN95fPoSPluSOZbL2P2kJ+3\nhlxED3tjnCZ09YnDAAAAVfwk8o3JZIR8k4J801j7teH7ks/eMOA6+jgS4zSif9ticQAAwPZSstN2\n+0gZTxZkvHKdObLPz6Mxr2wZ61tgAADgApb97nCsO0NvT+abRsQT68xxIPn8A0MtoqfHYpwm9LYW\niwMAALaXQ5FvSvaOkO/ignyLG8xzKjnHvO7+jdGEbvR7AgAAdDKJfFPywkgZS06JvXidObKvtY51\nCNNmPh3jNKKXtVgcAACwvbwR+aZkjJ3CRwvy3brBPE8k59g/xCIqGOPKlp80WRkAALCtXBH5pmSM\nU2TfU5Dv2CZzZeaY1ytKxriy5UyTlQEAANvOYuSakpMjZFuIiHPJfNPY+DqZq5NzfHOAddRwONo2\noUsxzvU8AADABe6eqNPkDeUXBfk+uslcJ5LzzOMhRWNc2TLGgVQAAMAFbmfkm5L7RsiX3cGcRsRT\nm8yVbeTeqL2ISu6Ktk3on7RZFgAAsN1kX/Uc45vJyfm6mXyZq0UeSM61u+YiKsr+FjXGWHfEAgAA\nF7hLIt+YvH+EfK8X5Ls0MV+mkZvXuzL3R9vd0D1tlgUAAGw32QOKjo+Q7WPJbNOIuD8xX7aRu73m\nIioquVqn73BKLgAAMIjPR74x2dk4266CbKeSc2ZfQZ5HrQ8p+u9tlgUAAGwnJY3ND0bId6wg3yQx\nX3a9r9RcREXfi3ZN6Ly+mgwAAGxxj0W+MWntUEG2g8k5v5Scb3+tRVSWfYW6xri+0ZoAAIBtZBL5\npuTqxtn2FGR7sWDeM4n5xjgVOONAtGtCnZQLAAAMIvut5FsjZDuVzLYUy6/bZmS/N72j1iIqezna\nNaKfbLQmAABgG9kb+aak9V2adxRkO1Aw71PJOXdUWENtpYcULUX+HxpWj6carQkAANhm3opcU/J8\n41yXJnNNI+Lxwrkzd4f+pvcKhnF7lDWTfxZlJw7PxrmYz0YcAADY4j4a+cYk+9prDZPIfcM5jYjT\nhXNfn5y3ZIe1pXOR/2+28rTbzxU8N43lb3MBAACqy568+veNc/0wmWsayzunJV5NzDmvhxRdHmXN\n5A2rnr8z8cy5iLho4HUAAADb1Kci18y0bsrem8w1jeXGqkT2+8qH+y5iIC9E/rc5t84c+2L9b0bv\ni7Y73wAAwDaT+U5yGsuv77ayUJDrSIf5/yY5944eaxhK6SFF/2WT+XbE8g7rzRHxttCAAgAAA/tG\n5JqZ0u8v+/p1Mtc0Ii7uMH/mKphjvVYwnFsj/9u4+xMAAJgrJTtrexvm+nhBri90mH9Pcu7r+yxi\nQNnDm1r/dwMAANjUQ5FrZlpeXzJJZprG8mFDXTyRmHteDykqucrm+EgZAQAA1lSyGzppmOu1ZKal\nHrky354+2nkFwyp5ZXn3SBkBAADW9HTkmpmWDdlNyUzTiLimY43s3aHzeHfmxZH/fX49UkYAAIA1\n7Yp8Q9PqBNWdBZn6vCr8cmL+Ez3mH9LpmM9dbAAAgE29Erlm5psNM2VOse37Su4kWeMTXRcxoL+L\nfBP60EgZAQAA1rQv8g1fK99NZppGxId61MleezJv92iW7GBPR8oIAACwrtcj18zc1ChPyXePz/es\nlXm19cmeNYZQ8krun4+UEQAAYE3vilwzc7phpuydmH1eyY3I7wRf2qPGEA6F3VAAAGALOxK5Zqbr\nibSlHkzmmUbE5T1rPZyocbZnjdpKDnCaxnJTDwAAMDcORK6ZebNRnkuSeaYR8WzPWguRuzv0jp51\najsZZY3oq+PEBAAAWFv2VNpW92cuJvNMo/9VJNm7Q3f0rFPTDVHWhE7DabkAAMAcyTY1LzTK81gy\nzzQiPlqhXuaV5CMV6tRU2oROI+K6UZICAACsIXsg0K4GWd6ZzDKN5ftO+8pefdLnWpjafh7dGtF5\nu3YGAADYprJ3Zz7TKE/LV3IjIr6TrDUvTdwkujWh0zHCAgAArLYQ+cavRSP2VDLLNCI+WKlmZv3z\ndHfob6NbE7o4RlgAAIDV7ohcE3NPgywfSGaZRsSLlWpmTwp+e6V6fWXa/3r4AAAQO0lEQVRfI15r\nzNs3rgAAwDaUfcVzKdrsho7xiulLiVrnKtbr63B0b0S/OkJeAACA3/HDyDUwX2+Q5TfJLDVfyV1I\n1vtupXp9ZfOuN3a2jwwAAPAPsq94ttgN/XAyyzTqnJI7c1uy5rwcUvRI9GtEAQAARpW9/uMLA+fY\nmcwxRDN1NlHvaOWaffRpQh1UBAAAjCq7G7oYw+8GHktmmUbE+yvW3ZeseX3Fmn2U7BoPvZMMAABQ\n7IXINS+3DJzjlmSOaSwfKlRT9pqYeXkt91z0a0SvaB8ZAABg2Z7INS5DnxQ7SeaYjZqyh/68ULlu\nV7ujXxNa+/cDAAAociRyjcsnBs5RssP3nyvX/liy7rzcHXo8+jWhvg8FAABG8/bINS5nBs7xeDLH\nNCKeGaD+6UTdeWneLo3+u6EPN08NAABw3puRa1zeN2CGy5IZhmoGswc1fXuA2l2ciP6N6MXNUwMA\nAETEu2L83dBJLN9Lmm2gdg6Q4cfJ2jsGqF3qk9G/CZ02Tw0AAHDeycg1LdcMmOH1ZIZpRPzdQBky\njfCJgWqXWIj+J+VOI+L51sEBAAAiIvZHrmk5O2CG25IZphFxdKAMB5L1rx2ofon7o85u6P7WwQEA\nACIi3opc03L1QPX3JutPY3nHcjJQjqPJDGPLfse6FdYCAABsQ++OXMNyesAMi8kM04i4cqAM2btD\nXxqofolXo04TOi/3oAIAANvMqRh3N/SXyfrTiPjeQBkiIr6azLB3wAwZl0f+99pseC0XAABoLvtt\n6FAn5d6YrD+N5YZ5SGcTGZYGzpCRyZkdAAAAzWXvDf3gALUvTtaejckAGWYmyQwPD5gh42+i7Dfb\naDzXODsAAEDsjlzDsjhA7YVY3mXNNk1DvRY882gyx46Bc2wk2yxnxyfaxgcAAIg4FrmG5boBaj+e\nrD2NiIcGqL9a5u7QIQ9ryng68r9ZZjzQNj4AALDdZa//GOKbyIPJ2tNYfnV4aNmrYw41yLKekutt\nsmPob24BAAB+x7ORa1Y+X7nunmTdWRM8qVx/LdlTexcaZFlP9mTjkjEPBy8BAADbRPa+zOkAdU8X\n1L68cv31zMvO7Ho+ukGuvgMAAKCJ70euSbmnct2S+0LvrVx7PdlXXj/aKM9aMt+vakQBAIC5lm1s\nar6KenOy5jQiDlesu5lsczyWkkOdNKIAAMBcuiFyDcoTFWtemqw5jeWrYiYVa29m3hrjlSbJfF2H\nb0QBAIAmzkbb3dBJRJxL1pzGctPaysXJTO9umGmlk8l8Xcdb7ZYCAABsV2+PXINytGLNw8ma04i4\nrWLdjGeSucbw4WS2PuPpZqsBAAC2rWORa1B2V6r3o2S9sZqizLeyL42QKxK5aoyDzVYDAABsS9kr\nW2q9rnl9st40Is5E+zs6s7vDlzXOFbHclLdoRMe8FxUAANgG/m/kmpNrK9Tan6w1G3sq1Cz102S2\n1nYnc/UdY+30AgAA20imOalxiuokyu69vKlCzS4yByi9OkKu7GFSfcdVrRYEAABsT5+KXHNye4Va\np5O1phHxVIV6XUyS+d7TONetyVx9x4OtFgQAAGxfra5seTVZZxrLDetY3yjelszYUrY5nsbyXatd\nm9DjEbGjzZIAAIDtKvu95nM96zyarDMbk571+sjcz/lK40xHE5lW7tQeKfj72TgaEW9rsxwAAGA7\nez5yTcquHjVuSdaYjat71Kohk/GahnluSGaaRsSnzz+zIyLuLXju3rATCgAANJC9suV4jxr/LVlj\nNr7Ro1YNN0YuZyvZ/0bTWPtqnati493oR8PBRAAAQEN3Rq7BOdBx/kuS88/GGx3r1PRabJ7z9YZ5\nXkjkmY2dm8z1tlhuOq8Kr+ACAAAjyVyjsthx7p2JuVeOszHe4UQrZbJ+olGWDyTzzF6tBQAAmGvX\nRa7BubHD3JMouys0s5vXwqWRy9qqYc7+hl3/sQAAAKCpN2OYpmshyq8PeXe/pVTz89g8a5/vZUv8\nKpFlNi5plAkAAKCziyLX4Pysw9xnknPPxl/2WEdtmftUb22Q48pEjtn4cYM8AAAAvT0ZuSZnR+G8\nx5LzzsZ9/ZZR1Z7IZe5zjU3WuWSWcw2yAAAA9Ja9DqT0BNtfJ+edjWd6rqO2W2PzzKca5PhJIsds\n7G2QBwAAoLdMwzWNiPcWzPlQcs7ZOFphHbUdj81zPzhwhuxhSS2yAAAAVJM5SOh0wXyfS8y3cpys\nsYjKsrvE+wbOkflG1Su5AADAlvJfI9fo3JSc72ByvpUN1DzcFbra/4jNsy8NnOEHiQxeyQUAALac\n16Jew7U/MdfKsRjz2YRGRLwcm+d/ZMD6Ja/kfnfAHAAAAFVdErlG53uJuXYl51rZ3E7qLaWqHZFb\nw+UD1V+I/JU3Ja9MAwAAjGoh8t8fbrZrOSmYazZ2V11NXbdFnd+lq0eT9b2SCwAAbCmHI9foPJ+Y\n60Ryrtl4e8V1DCHTVB8eqPblidqzcddAGQAAAKp7JPLNzp5N5iq9K/Syukup7l2RW8fdA9Qu2aU+\nMUB9AACAQXwq8k3jZleCPFYw1zQirqm7lEG8Grm1XDVA7R8ma09j+ZtcAACAubc7yhrHjV4/PVQ4\n1+eqr6a+HTFeI1jySu6tlWsDAAAMZinKmscn1pmn9K7QQ4Ospr57Iree2veHTmL5Kpu+/zgAAAAw\nV45GWfM4jYivrjHPBwrn+NFQCxpAthk8Vrnu88m6XskFAAC2jFuivAmdRsTVq+bZX/j8s4OtqL4D\nkV/XwxXrluwu/8+KdQEAAAYziW5N6DR+957M0nneHHZZ1b0U+bV9tFLNkt/UK7kAAMCWcSq6N6Iz\nkyj7vnQpfreJnXcLUfa7TCrVLflvs5V+TwAAYBsr/Z5zvUY0++3kbOwedlnVlZ4AXMPDBfWuq1QT\nAABgcKWn5K4cp87PcbrwuQPDL6u6s5Ff35kK9a4sqPebCvUAAACa+GT02w19MSKOFD7z101WVtck\nytb4UuN6k571AAAAmumzGzqNiBOFf/+DNsuq7rtRts7P9Kx3pqBWrUORAAAABndZ9GtCS8dWPtG1\ntGG/uEetJwvqvNCjDgAAQHNvRrsm9HSjNQ1hV5Svt6sbCmos9agDAADQXOlVJH3GVrumZbV7o3y9\nXewtrLO/Yx0AAIBRfCnaNaKTRmsayrkoW++bHWqU/sPAdzqvBgAAYCQlh+H0GVvtrtC1lK65y4FM\nbxXMf2qdOQDg//v9sQMAwCqTiPinDer8p4i4v0GdIV3b4Zk7C//+FxHxzwv+/l8Vzg8AADC6L8fw\nO6FXNFvNsF6O8rWX+ELh3Ht7rQYAAGAkp2LYJvRgu6UMbjGGa0T3F877pd6rAQAAGMHQp+V+rt1S\nmihd/2Jy3kmU3U36TJXVAAAAjOBjMVwTeqjhOlq4Isp/g9eSc58omHMr38EKAAAQh2OYJvTuloto\n5KEo/x2+mpj3sYL5tvodrAAAAIM0oU82XUE7J6P8t9i5yZylO9IOJwIAALa090X9JvT1pitoq+Qb\nztnYyJ7CuT5QdTUAAAAjeCTqNqFn48J+bbT091jaYK6FWP69snP9oPpqAAAARnA66jWhS7F88uuF\n6oNR/psc22C+XxTM85vqqwEAABhJzd3Q/9g4e2sPRvlv8tA6c91WMMfZQVYDAAAwgpr3h364cfYx\nvBTlv8v715jn0sI5dg21IAAAgNZ2RJ0m9N62sUezGOW/zWqTKDvw6MBgqwEAABhJjUb0ba1Dj6TL\nb7NayTe5XxpuKQBsR78/dgAAOO/c2AG2iIs7PPPWqv/9uYj4Z8lnn47lV3gBAAAuOC9G/x3R7eBg\nlP8uT614/m8LnrvQr8ABAAC2uRuiXxP6ZPvIo/hZlP82B88/e0Xhcw4nAgAALnh97hL9SPu4ozgZ\n5b/NJCIuKXzmxlYLAgAAGNO7olsT+tgYYUfS5feZFP79881WAwAAMAe+EuWN1kWjJG2vy/ehZ6Ls\nmpalZqsBAACYI9nvRZ+N7XNlS+mu5srGsuTv39NoPQAAAHPnooh4ItZvmP40tteJrkejWyNaMu5v\nthoAtrXfGzsAAGxiIZab0osi4khEPHp+bCeXRcTnBq5xOiL+xcA1AAAA2CJ+G8Pvhk6arQYAAIC5\nN3QTemW7pQAAADDv9sewTeh2e80ZAACATdwRwzWhJxquAwAAgC3ixfBdKAAAAA0di2Ga0Pe2XAQA\nAABbxxCN6KGmKwAAAGBLeTnqNqHPt40PAP/Y748dAADY0LmKcy1GxL+uOB8AdKIRBYD59ljFuf5d\nxbkAoDONKADMt/9daZ6lqNvUAgAAcIFaiDrfhj7eOjgArMeOKADMtyMRcbLCPHdUmAMAqtCIAsD8\nu7fCHHdXmAMAAIBtYkdEnIjur+X+XfPEAAAAbHl/GN2a0KOx/J0pAAAAFPvTKGtCj0TE28YICgAA\nwIXjD2O5wdysCb037IQCAABQyUJEfCSWm82VTemzsfw96HvGiQUAAMB2sWPsAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAW9D/A4B7ViPrMDeYAAAAAElF\nTkSuQmCC\n"<br/>
      },<br/>
      "field_type": "signature",<br/>
      "label": "Naamloos",<br/>
      "required": true<br/>
    }`<br/>
  <br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add forms [POST]<br/>
<br/>
<br/>
+ Request Correct object data posted. `response` will contain the amount of forms synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"name":"Checklist","data":"{\"fields\":[{\"label\":\"Type zonnepaneel\",\"field_type\":\"radio\",\"required\":true,\"field_options\":{\"options\":[{\"label\":\"a\",\"checked\":false},{\"label\":\"b\",\"checked\":false},{\"label\":\"c\",\"checked\":false}]},\"cid\":\"c2\"}]}","template":""},{"name":"Controle lijst","data":"{\"fields\":[{\"label\":\"Jaartal\",\"field_type\":\"text\",\"required\":true,\"field_options\":{\"size\":\"small\",\"value\":\"\"},\"cid\":\"c2\"},{\"label\":\"Staat van het huis goed\",\"field_type\":\"checkboxes\",\"required\":true,\"field_options\":{\"options\":[{\"label\":\"Ja\",\"checked\":false},{\"label\":\"Nee\",\"checked\":false},{\"label\":\"Weet ik niet\",\"checked\":false}]},\"cid\":\"c6\"}]}","template":""},{"name":"Eigen form","data":"{\"fields\":[{\"label\":\"Type pomp\",\"field_type\":\"checkboxes\",\"required\":true,\"field_options\":{\"options\":[{\"label\":\"type A\",\"checked\":false},{\"label\":\"type B\",\"checked\":false},{\"label\":\"type C\",\"checked\":false}]},\"cid\":\"c2\"},{\"label\":\"Serienummer\",\"field_type\":\"text\",\"required\":true,\"field_options\":{\"size\":\"small\",\"value\":\"\"},\"cid\":\"c6\"},{\"label\":\"Dropdown\",\"field_type\":\"dropdown\",\"required\":true,\"field_options\":{\"options\":[{\"label\":\"A\",\"checked\":false},{\"label\":\"B\",\"checked\":false}],\"include_blank_option\":false},\"cid\":\"c10\"}]}","template":""}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": 3<br/>
            }<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
<br/>
            [{"data":"{\"fields\":[{\"label\":\"Type zonnepaneel\",\"field_type\":\"radio\",\"required\":true,\"field_options\":{\"options\":[{\"label\":\"a\",\"checked\":false},{\"label\":\"b\",\"checked\":false},{\"label\":\"c\",\"checked\":false}]},\"cid\":\"c2\"}]}","template":""},{"name":"Controle lijst","data":"{\"fields\":[{\"label\":\"Jaartal\",\"field_type\":\"text\",\"required\":true,\"field_options\":{\"size\":\"small\",\"value\":\"\"},\"cid\":\"c2\"},{\"label\":\"Staat van het huis goed\",\"field_type\":\"checkboxes\",\"required\":true,\"field_options\":{\"options\":[{\"label\":\"Ja\",\"checked\":false},{\"label\":\"Nee\",\"checked\":false},{\"label\":\"Weet ik niet\",\"checked\":false}]},\"cid\":\"c6\"}]}","template":""},{"name":"Eigen form","data":"{\"fields\":[{\"label\":\"Type pomp\",\"field_type\":\"checkboxes\",\"required\":true,\"field_options\":{\"options\":[{\"label\":\"type A\",\"checked\":false},{\"label\":\"type B\",\"checked\":false},{\"label\":\"type C\",\"checked\":false}]},\"cid\":\"c2\"},{\"label\":\"Serienummer\",\"field_type\":\"text\",\"required\":true,\"field_options\":{\"size\":\"small\",\"value\":\"\"},\"cid\":\"c6\"},{\"label\":\"Dropdown\",\"field_type\":\"dropdown\",\"required\":true,\"field_options\":{\"options\":[{\"label\":\"A\",\"checked\":false},{\"label\":\"B\",\"checked\":false}],\"include_blank_option\":false},\"cid\":\"c10\"}]}","template":""}]<br/>
<br/>
+ Response 200 (application/json)<br/>
 "<br/>
    + Body<br/>
<br/>
            {"code":2301,"messages":["Required field missing: name"],"response":null}<br/>
              <br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{""data":"{\"fields\":[{\"label\":\"Type zonnepaneel\",\"field_type\":\"radio\",\"required\":true,\"field_options\":{\"options\":[{\"label\":\"a\",\"checked\":false},{\"label\":\"b\",\"checked\":false},{\"label\":\"c\",\"checked\":false}]},\"cid\":\"c2\"}]}","template":""},{"name":"Controle lijst","data":"{\"fields\":[{\"label\":\"Jaartal\",\"field_type\":\"text\",\"required\":true,\"field_options\":{\"size\":\"small\",\"value\":\"\"},\"cid\":\"c2\"},{\"label\":\"Staat van het huis goed\",\"field_type\":\"checkboxes\",\"required\":true,\"field_options\":{\"options\":[{\"label\":\"Ja\",\"checked\":false},{\"label\":\"Nee\",\"checked\":false},{\"label\":\"Weet ik niet\",\"checked\":false}]},\"cid\":\"c6\"}]}","template":""},{"name":"Eigen form","data":"{\"fields\":[{\"label\":\"Type pomp\",\"field_type\":\"checkboxes\",\"required\":true,\"field_options\":{\"options\":[{\"label\":\"type A\",\"checked\":false},{\"label\":\"type B\",\"checked\":false},{\"label\":\"type C\",\"checked\":false}]},\"cid\":\"c2\"},{\"label\":\"Serienummer\",\"field_type\":\"text\",\"required\":true,\"field_options\":{\"size\":\"small\",\"value\":\"\"},\"cid\":\"c6\"},{\"label\":\"Dropdown\",\"field_type\":\"dropdown\",\"required\":true,\"field_options\":{\"options\":[{\"label\":\"A\",\"checked\":false},{\"label\":\"B\",\"checked\":false}],\"include_blank_option\":false},\"cid\":\"c10\"}]}","template":""}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1009,<br/>
              "messages": [<br/>
                "Unable to parse body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1008,<br/>
              "messages": [<br/>
                "Unable to fetch body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
### Get forms [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":200,"messages":[],"response":[{"name":"Checklist","data":"{\"fields\":[{\"label\":\"Type zonnepaneel\",\"field_type\":\"radio\",\"required\":true,\"field_options\":{\"options\":[{\"label\":\"a\",\"checked\":false},{\"label\":\"b\",\"checked\":false},{\"label\":\"c\",\"checked\":false}]},\"cid\":\"c2\"}]}","template":""},{"name":"Controle lijst","data":"{\"fields\":[{\"label\":\"Jaartal\",\"field_type\":\"text\",\"required\":true,\"field_options\":{\"size\":\"small\",\"value\":\"\"},\"cid\":\"c2\"},{\"label\":\"Staat van het huis goed\",\"field_type\":\"checkboxes\",\"required\":true,\"field_options\":{\"options\":[{\"label\":\"Ja\",\"checked\":false},{\"label\":\"Nee\",\"checked\":false},{\"label\":\"Weet ik niet\",\"checked\":false}]},\"cid\":\"c6\"}]}","template":""},{"name":"Eigen form","data":"{\"fields\":[{\"label\":\"Type pomp\",\"field_type\":\"checkboxes\",\"required\":true,\"field_options\":{\"options\":[{\"label\":\"type A\",\"checked\":false},{\"label\":\"type B\",\"checked\":false},{\"label\":\"type C\",\"checked\":false}]},\"cid\":\"c2\"},{\"label\":\"Serienummer\",\"field_type\":\"text\",\"required\":true,\"field_options\":{\"size\":\"small\",\"value\":\"\"},\"cid\":\"c6\"},{\"label\":\"Dropdown\",\"field_type\":\"dropdown\",\"required\":true,\"field_options\":{\"options\":[{\"label\":\"A\",\"checked\":false},{\"label\":\"B\",\"checked\":false}],\"include_blank_option\":false},\"cid\":\"c10\"}]}","template":""}]}<br/>
<br/>
## suppliers [/suppliers/{?token,software_token}]<br/>
<br/>
This api is used to sync suppliers with WorkorderApp.<br/>
<br/>
Each supplier record can contain the following data:<br/>
<br/>
| Parameter                 | Description                                                                                                               | Required | Type (size)   |<br/>
|---------------------------|---------------------------------------------------------------------------------------------------------------------------|----------|---------------|<br/>
| sup_code                  | Unique code of the supplier. Used as reference for other entities                                                         | Y        | Varchar (255) |<br/>
| sup_name                  | Supplier name                                                                                                             | Y        | Varchar (255) |<br/>
| sup_image                 | Url of the image name. POST: An external url should be provided.  GET: You will receive a workorderapp url.               | N        | Varchar (255)      |<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add suppliers [POST]<br/>
<br/>
<br/>
+ Request Correct supplier data posted. `response` will contain the amount of suppliers synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"sup_code":"001","sup_name":"Pirelli","sup_image":""},{"sup_code":"002","sup_name":"Volkswagen","sup_image":""}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": 2<br/>
            }<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
<br/>
            [{"sup_name":"Pirelli","sup_image":""},{"sup_code":"002","sup_name":"Volkswagen","sup_image":""}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 2001,<br/>
              "messages": [<br/>
                "Required field missing: sup_code"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
  <br/>
              <br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"sup_code"": "001","sup_name": "Pirelli","sup_image":""},{"sup_code": "002","sup_name": "Volkswagen","sup_image":""}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1009,<br/>
              "messages": [<br/>
                "Unable to parse body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1008,<br/>
              "messages": [<br/>
                "Unable to fetch body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
### Get suppliers [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [<br/>
                {<br/>
                  "sup_code": "001",<br/>
                  "sup_name": "Pirelli",<br/>
                  "sup_image":""<br/>
                },<br/>
                {<br/>
                  "sup_code": "002",<br/>
                  "sup_name": "Volkswagen",<br/>
                  "sup_image":""<br/>
                }<br/>
              ]<br/>
            }<br/>
                  <br/>
            <br/>
## objects [/objects/{?token,software_token}]<br/>
<br/>
This api is used to sync objects with WorkorderApp.<br/>
<br/>
Each object record can contain the following data:<br/>
<br/>
| Parameter                 | Description                                                                                                               | Required | Type (size)   |<br/>
|---------------------------|---------------------------------------------------------------------------------------------------------------------------|----------|---------------|<br/>
| obj_code                  | Unique code of the object. Used as reference for other entities                                                           | Y        | Varchar (255) |<br/>
| obj_sup_code              | Supplier code. Used as reference to supplier entity                                                                       | N        | Varchar (255) |<br/>
| obj_debiteur_nummer       | Debtor number. Used as reference to customer clients.                                                                     | Y        | Varchar (255) |<br/>
| obj_adr_code              | Address code. Used as a reference to the addres of a customer client.                                                     | N        | Varchar (255) |<br/>
| obj_obj_code              | Parent object code.                                                                                                       | N        | Varchar (255) |<br/>
| obj_image                 | Url of the image name. POST: An external url should be provided.  GET: You will receive a workorderapp url.               | N        | Varchar (255) |<br/>
| obj_description           | Description of the object                                                                                                 | Y        | Varchar (255) |<br/>
| obj_price                 | Price of the object                                                                                                       | N        | Decimal (7,2) |<br/>
| obj_floor_level           | Floor level of the object                                                                                                 | N        | Int (10)      |<br/>
| obj_location              | Textual description of the location of the object                                                                         | N        | Varchar (255) |<br/>
| obj_latitude              | Latitude of the location of the object                                                                                    | N        | Float (10,6)  |<br/>
| obj_longitude             | Longitude of the location of the object                                                                                   | N        | Float (10,6)  |<br/>
| obj_type                  | Type                                                                                                                      | N        | Varchar (255) |<br/>
| obj_model                 | Model                                                                                                                     | N        | Varchar (255) |<br/>
| obj_brand                 | Brand                                                                                                                     | N        | Varchar (255) |<br/>
| obj_date_warranty_expires | Expiration date of the warranty                                                                                           | N        | Varchar (255) |<br/>
| obj_serialnumber          | Serialnumber of the object                                                                                                | N        | Varchar (255) |<br/>
| obj_date_last_inspection  | Date of last inspection                                                                                                   | N        | Varchar (255) |<br/>
| obj_date_installation     | Date of installation                                                                                                      | N        | Varchar (255) |<br/>
| obj_freefield_1           |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_2           |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_3           |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_4           |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_5           |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_6           |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_7           |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_8           |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_9           |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_10          |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_11          |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_12          |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_13          |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_14          |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_15          |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_16          |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_17          |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_18          |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_19          |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_freefield_20          |                                                                                                                           | N        | Varchar (255) |<br/>
| obj_order                 | Sort order of an object                                                                                                   | N        | Int (10)      |<br/>
| obj_created               | Timestamp of creating                                                                                                     | N        | DateTime      |<br/>
| obj_modified              | Timestamp of modifying                                                                                                    | N        | DateTime      |<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add object [POST]<br/>
<br/>
<br/>
+ Request Correct object data posted. `response` will contain the amount of objects synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"obj_code":"Object 22323","obj_sup_code":"gfgd","obj_debiteur_nummer":"4_548a427a-45e8-4f05-9eff-36c8dd742942","obj_adr_code":"","obj_obj_code":"ghd","obj_image":"no-image.png","obj_description":"Object 2","obj_price":"0.00","obj_floor_level":"0","obj_location":"","obj_latitude":null,"obj_longitude":null,"obj_type":"","obj_model":"","obj_brand":"sdfds","obj_date_warranty_expires":"2017-03-01","obj_serialnumber":"dsfs","obj_date_last_inspection":"2017-03-01","obj_date_installation":"2017-03-01","obj_freefield_1":"Merk x","obj_freefield_2":"Model y ","obj_freefield_3":"11-12-2016","obj_freefield_4":"","obj_freefield_5":"","obj_freefield_6":"","obj_freefield_7":"","obj_freefield_8":"","obj_freefield_9":"","obj_freefield_10":"","obj_freefield_11":"","obj_freefield_12":"","obj_freefield_13":"","obj_freefield_14":"","obj_freefield_15":"","obj_freefield_16":"","obj_freefield_17":"","obj_freefield_18":"","obj_freefield_19":"12","obj_freefield_20":"","obj_order":""}]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": 1<br/>
            }<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
<br/>
            [{"obj_sup_code":"gfgd","obj_debiteur_nummer":"4_548a427a-45e8-4f05-9eff-36c8dd742942","obj_adr_code":"","obj_obj_code":"ghd","obj_image":"no-image.png","obj_description":"Object 2","obj_price":"0.00","obj_floor_level":"0","obj_location":"","obj_latitude":null,"obj_longitude":null,"obj_type":"","obj_model":"","obj_brand":"sdfds","obj_date_warranty_expires":"2017-03-01","obj_serialnumber":"dsfs","obj_date_last_inspection":"2017-03-01","obj_date_installation":"2017-03-01","obj_freefield_1":"Merk x","obj_freefield_2":"Model y ","obj_freefield_3":"11-12-2016","obj_freefield_4":"","obj_freefield_5":"","obj_freefield_6":"","obj_freefield_7":"","obj_freefield_8":"","obj_freefield_9":"","obj_freefield_10":"","obj_freefield_11":"","obj_freefield_12":"","obj_freefield_13":"","obj_freefield_14":"","obj_freefield_15":"","obj_freefield_16":"","obj_freefield_17":"","obj_freefield_18":"","obj_freefield_19":"12","obj_freefield_20":"","obj_order":""}]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1901,<br/>
              "messages": [<br/>
                "Required field missing: obj_code"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
  <br/>
              <br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"obj_code"":"Object 22323","obj_sup_code":"gfgd","obj_debiteur_nummer":"4_548a427a-45e8-4f05-9eff-36c8dd742942","obj_adr_code":"","obj_obj_code":"ghd","obj_image":"no-image.png","obj_description":"Object 2","obj_price":"0.00","obj_floor_level":"0","obj_location":"","obj_latitude":null,"obj_longitude":null,"obj_type":"","obj_model":"","obj_brand":"sdfds","obj_date_warranty_expires":"2017-03-01","obj_serialnumber":"dsfs","obj_date_last_inspection":"2017-03-01","obj_date_installation":"2017-03-01","obj_freefield_1":"Merk x","obj_freefield_2":"Model y ","obj_freefield_3":"11-12-2016","obj_freefield_4":"","obj_freefield_5":"","obj_freefield_6":"","obj_freefield_7":"","obj_freefield_8":"","obj_freefield_9":"","obj_freefield_10":"","obj_freefield_11":"","obj_freefield_12":"","obj_freefield_13":"","obj_freefield_14":"","obj_freefield_15":"","obj_freefield_16":"","obj_freefield_17":"","obj_freefield_18":"","obj_freefield_19":"12","obj_freefield_20":"","obj_order":""}]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1009,<br/>
              "messages": [<br/>
                "Unable to parse body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1008,<br/>
              "messages": [<br/>
                "Unable to fetch body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
### Get objects [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [{"obj_code":"Object 2","obj_sup_code":"gfgd","obj_debiteur_nummer":"4_548a427a-45e8-4f05-9eff-36c8dd742942","obj_adr_code":"","obj_obj_code":"ghd","obj_image":"no-image.png","obj_description":"Object 2","obj_price":"0.00","obj_floor_level":"0","obj_location":"","obj_latitude":null,"obj_longitude":null,"obj_type":"","obj_model":"","obj_brand":"sdfds","obj_date_warranty_expires":"2017-03-01","obj_serialnumber":"dsfs","obj_date_last_inspection":"2017-03-01","obj_date_installation":"2017-03-01","obj_freefield_1":"Merk x","obj_freefield_2":"Model y ","obj_freefield_3":"11-12-2016","obj_freefield_4":"","obj_freefield_5":"","obj_freefield_6":"","obj_freefield_7":"","obj_freefield_8":"","obj_freefield_9":"","obj_freefield_10":"","obj_freefield_11":"","obj_freefield_12":"","obj_freefield_13":"","obj_freefield_14":"","obj_freefield_15":"","obj_freefield_16":"","obj_freefield_17":"","obj_freefield_18":"","obj_freefield_19":"12","obj_freefield_20":"","obj_created":"0000-00-00 00:00:00","obj_modified":"2017-03-02 11:10:44"},{"obj_code":"Object 1","obj_sup_code":"","obj_debiteur_nummer":"4_548a427a-45e8-4f05-9eff-36c8dd742942","obj_adr_code":"","obj_obj_code":"","obj_image":"no-image.png","obj_description":"Object 1","obj_price":"0.00","obj_floor_level":"0","obj_location":"","obj_latitude":null,"obj_longitude":null,"obj_type":"","obj_model":"","obj_brand":"","obj_date_warranty_expires":"","obj_serialnumber":"","obj_date_last_inspection":"","obj_date_installation":"","obj_freefield_1":"","obj_freefield_2":"","obj_freefield_3":"","obj_freefield_4":"","obj_freefield_5":"","obj_freefield_6":"","obj_freefield_7":"","obj_freefield_8":"","obj_freefield_9":"","obj_freefield_10":"","obj_freefield_11":"","obj_freefield_12":"","obj_freefield_13":"","obj_freefield_14":"","obj_freefield_15":"","obj_freefield_16":"","obj_freefield_17":"","obj_freefield_18":"","obj_freefield_19":"","obj_freefield_20":"","obj_order":"","obj_created":"0000-00-00 00:00:00","obj_modified":"0000-00-00 00:00:00"}]<br/>
            }<br/>
## objects/changed [/objects/changed/{?token,software_token,obj_code}]<br/>
<br/>
This api is used to fetch changed objects. A change can be made from the app. Once the information is processed the api can be called with the obj_code parameter. The changed indicator will be set to 0 so the record won't be shown again.<br/>
<br/>
### Get changed objects [GET]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [{"obj_code":"Object 2","obj_sup_code":"gfgd","obj_debiteur_nummer":"4_548a427a-45e8-4f05-9eff-36c8dd742942","obj_adr_code":"","obj_obj_code":"ghd","obj_image":"no-image.png","obj_description":"Object 2","obj_price":"0.00","obj_floor_level":"0","obj_location":"","obj_latitude":null,"obj_longitude":null,"obj_type":"","obj_model":"","obj_brand":"sdfds","obj_date_warranty_expires":"2017-03-01","obj_serialnumber":"dsfs","obj_date_last_inspection":"2017-03-01","obj_date_installation":"2017-03-01","obj_freefield_1":"Merk x","obj_freefield_2":"Model y ","obj_freefield_3":"11-12-2016","obj_freefield_4":"","obj_freefield_5":"","obj_freefield_6":"","obj_freefield_7":"","obj_freefield_8":"","obj_freefield_9":"","obj_freefield_10":"","obj_freefield_11":"","obj_freefield_12":"","obj_freefield_13":"","obj_freefield_14":"","obj_freefield_15":"","obj_freefield_16":"","obj_freefield_17":"","obj_freefield_18":"","obj_freefield_19":"12","obj_freefield_20":"","obj_created":"0000-00-00 00:00:00","obj_modified":"2017-03-02 11:10:44"},{"obj_code":"Object 1","obj_sup_code":"","obj_debiteur_nummer":"4_548a427a-45e8-4f05-9eff-36c8dd742942","obj_adr_code":"","obj_obj_code":"","obj_image":"no-image.png","obj_description":"Object 1","obj_price":"0.00","obj_floor_level":"0","obj_location":"","obj_latitude":null,"obj_longitude":null,"obj_type":"","obj_model":"","obj_brand":"","obj_date_warranty_expires":"","obj_serialnumber":"","obj_date_last_inspection":"","obj_date_installation":"","obj_freefield_1":"","obj_freefield_2":"","obj_freefield_3":"","obj_freefield_4":"","obj_freefield_5":"","obj_freefield_6":"","obj_freefield_7":"","obj_freefield_8":"","obj_freefield_9":"","obj_freefield_10":"","obj_freefield_11":"","obj_freefield_12":"","obj_freefield_13":"","obj_freefield_14":"","obj_freefield_15":"","obj_freefield_16":"","obj_freefield_17":"","obj_freefield_18":"","obj_freefield_19":"","obj_freefield_20":"","obj_order":"","obj_created":"0000-00-00 00:00:00","obj_modified":"0000-00-00 00:00:00"}]<br/>
            }<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
    + obj_code (string,optional) ... Code of the object that is succesfully updated in the external software.<br/>
<br/>
## object [/object/?token={token}&software_token={software_token}&key={key}&value={value}]<br/>
<br/>
This api is used to fetch objects based on a filter. Filters can be given by adding a key and values array to the URL.<br/>
Adding a single filter: &key=key1&value=value1<br/>
Adding multiple filters: &key[]=key1&value[]=value1&key[]=key2&value[]=value2<br/>
<br/>
### Get objects by filter [GET]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [{"obj_code":"Object 2","obj_sup_code":"gfgd","obj_debiteur_nummer":"4_548a427a-45e8-4f05-9eff-36c8dd742942","obj_adr_code":"","obj_obj_code":"ghd","obj_image":"no-image.png","obj_description":"Object 2","obj_price":"0.00","obj_floor_level":"0","obj_location":"","obj_latitude":null,"obj_longitude":null,"obj_type":"","obj_model":"","obj_brand":"sdfds","obj_date_warranty_expires":"2017-03-01","obj_serialnumber":"dsfs","obj_date_last_inspection":"2017-03-01","obj_date_installation":"2017-03-01","obj_freefield_1":"Merk x","obj_freefield_2":"Model y ","obj_freefield_3":"11-12-2016","obj_freefield_4":"","obj_freefield_5":"","obj_freefield_6":"","obj_freefield_7":"","obj_freefield_8":"","obj_freefield_9":"","obj_freefield_10":"","obj_freefield_11":"","obj_freefield_12":"","obj_freefield_13":"","obj_freefield_14":"","obj_freefield_15":"","obj_freefield_16":"","obj_freefield_17":"","obj_freefield_18":"","obj_freefield_19":"12","obj_freefield_20":"","obj_created":"0000-00-00 00:00:00","obj_modified":"2017-03-02 11:10:44"},{"obj_code":"Object 1","obj_sup_code":"","obj_debiteur_nummer":"4_548a427a-45e8-4f05-9eff-36c8dd742942","obj_adr_code":"","obj_obj_code":"","obj_image":"no-image.png","obj_description":"Object 1","obj_price":"0.00","obj_floor_level":"0","obj_location":"","obj_latitude":null,"obj_longitude":null,"obj_type":"","obj_model":"","obj_brand":"","obj_date_warranty_expires":"","obj_serialnumber":"","obj_date_last_inspection":"","obj_date_installation":"","obj_freefield_1":"","obj_freefield_2":"","obj_freefield_3":"","obj_freefield_4":"","obj_freefield_5":"","obj_freefield_6":"","obj_freefield_7":"","obj_freefield_8":"","obj_freefield_9":"","obj_freefield_10":"","obj_freefield_11":"","obj_freefield_12":"","obj_freefield_13":"","obj_freefield_14":"","obj_freefield_15":"","obj_freefield_16":"","obj_freefield_17":"","obj_freefield_18":"","obj_freefield_19":"","obj_freefield_20":"","obj_order":"","obj_created":"0000-00-00 00:00:00","obj_modified":"0000-00-00 00:00:00"}]<br/>
            }<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
    + key (array,optional) ... Filter column, can be any of the allowed parameters.<br/>
    + value (array,optional) ... Filter value.<br/>
<br/>
## parts - DEPRECATED [/parts/{?token,software_token}]<br/>
<br/>
This api is now deprecated. Use materials to register the parts of certain objects.<br/>
<br/>
<br/>
This api is used to sync parts with WorkorderApp.<br/>
<br/>
Each part record can contain the following data:<br/>
<br/>
| Parameter                 | Description                                                                                                               | Required | Type (size)   |<br/>
|---------------------------|---------------------------------------------------------------------------------------------------------------------------|----------|---------------|<br/>
| prt_code                  | Unique code of the parts. Used as reference for other entities                                                         | Y        | Varchar (255) |<br/>
| prt_name                  | Part name/description name                                                                                                             | Y        | Varchar (255) |<br/>
| prt_sup_code              | Supplier code                                                                                                             | Y        | Varchar (255) |<br/>
| prt_value                 | Value of a parts                                                                                                             | Y        | Varchar (255) |<br/>
| prt_image                 | Url of the image name. POST: An external url should be provided.  GET: You will receive a workorderapp url.     | N        | Varchar (255)      |<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add parts [POST]<br/>
<br/>
<br/>
+ Request Correct parts data posted. `response` will contain the amount of parts synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"prt_code":"PRT001","prt_name":"Remschijf","prt_sup_code":"001","prt_value":"80.00","prt_image":""}]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {"code":200,"messages":[],"response":1}<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
        <br/>
            [{"prt_name":"Remschijf","prt_sup_code":"001","prt_value":"80.00","prt_image":""}]<br/>
        <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":2101,"messages":["Required field missing: prt_code"],"response":null}<br/>
              <br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"prt_code"":"PRT001","prt_name":"Remschijf","prt_sup_code":"001","prt_value":"80.00","prt_image":""}]            <br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1009,"messages":["Unable to parse body"],"response":null}<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1008,<br/>
              "messages": [<br/>
                "Unable to fetch body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
### Get parts [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [<br/>
                {<br/>
                  "prt_code": "PRT001",<br/>
                  "prt_name": "Remschijf",<br/>
                  "prt_sup_code": "001",<br/>
                  "prt_value": "80.00",<br/>
                  "prt_image": ""<br/>
                }<br/>
              ]<br/>
            }<br/>
            <br/>
## object_parts [/object_parts/{?token,software_token}]<br/>
<br/>
This api is used to sync object parts with WorkorderApp.<br/>
<br/>
The result can be filtered by using the advanced filter. As described in the introduction section. Allowed columns: `opr_obj_code` `opr_prt_code` `opr_serial_number`<br/>
<br/>
<br/>
Each object_part record can contain the following data:<br/>
<br/>
| Parameter                         | Description                                           | Required | Type (size)   |<br/>
|-----------------------------------|-------------------------------------------------------|----------|---------------|<br/>
| opr_obj_code                      | Object code                                           | Y        | Varchar (255) |<br/>
| opr_prt_code                      | Object part (Artikelcode from items in materials)     | Y        | Varchar (255) |<br/>
| opr_serial_number                 | Serial number of parts used in object                 | N        | Varchar (255) |<br/>
| opr_description                   | Description of a part                                 | N        | Varchar (255) |<br/>
| opr_amount                        | Amount of parts used in object                        | Y        | Int (10)      |<br/>
| opr_timestamp_installation        | Date of installing (Y-m-d)                            | N        | Date       |<br/>
| opr_warranty_months               | Amount of months, used to calculate expiration date.  | N        | Int (10)      |<br/>
| opr_timestamp_warranty_expires    | Warranty expiration date, automatically calculated based on installation date and the warranty months    | N        | Varchar (255)      |<br/>
| val_value_1                       | Freefield value 1                                     | N        | Varchar (255)      |<br/>
| val_value_2  - val_value_20       | Freefield value 2  till 20                            | N        | Varchar (255)      |<br/>
 <br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add object parts [POST]<br/>
<br/>
<br/>
+ Request Correct object parts data posted. `response` will contain the amount of objects synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [<br/>
                {<br/>
                    "opr_obj_code": "Object 1",<br/>
                    "opr_prt_code": "001",<br/>
                    "opr_serial_number": "65644456",<br/>
                    "opr_description" :"",<br/>
                    "opr_timestamp_installation": "2018-10-11",<br/>
                    "opr_warranty_months": "24",<br/>
                    "opr_amount": "4",<br/>
                    "val_value_1": "Free field 1 value",<br/>
                    "val_value_2": "Free field 1 value"<br/>
                }<br/>
            ]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {"code":200,"messages":[],"response":1}<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
        <br/>
            [<br/>
                {<br/>
                    "opr_prt_code": "001",<br/>
                    "opr_amount": "4"<br/>
                }<br/>
            ]<br/>
        <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 2201,<br/>
              "messages": [<br/>
                "Required field missing: opr_obj_code"<br/>
              ],<br/>
              "response": null<br/>
            }  <br/>
            <br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [<br/>
                {<br/>
                  "opr_obj_code"": "Object 1",<br/>
                  "opr_prt_code": "001",<br/>
                  "opr_amount": "4"<br/>
                }<br/>
            ]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1009,"messages":["Unable to parse body"],"response":null}<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1008,<br/>
              "messages": [<br/>
                "Unable to fetch body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
### Get object parts [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [<br/>
                 {<br/>
                    "opr_obj_code": "Object 1",<br/>
                    "opr_prt_code": "001",<br/>
                    "opr_serial_number": "65644456",<br/>
                    "opr_description": "",<br/>
                    "opr_timestamp_installation": "2018-10-11",<br/>
                    "opr_warranty_months": "24",<br/>
                    "opr_timestamp_warranty_expires": "2020-10-11",<br/>
                    "opr_amount": "4",<br/>
                    "val_value_1": "Free field 1 value",<br/>
                    "val_value_2": "Free field 1 value"<br/>
                    "val_value_3": null,<br/>
                    "val_value_4": null,<br/>
                    "val_value_5": null,<br/>
                    "val_value_6": null,<br/>
                    "val_value_7": null,<br/>
                    "val_value_8": null,<br/>
                    "val_value_9": null,<br/>
                    "val_value_10": null,<br/>
                    "val_value_11": null,<br/>
                    "val_value_12": null,<br/>
                    "val_value_13": null,<br/>
                    "val_value_14": null,<br/>
                    "val_value_15": null,<br/>
                    "val_value_16": null,<br/>
                    "val_value_17": null,<br/>
                    "val_value_18": null,<br/>
                    "val_value_19": null,<br/>
                    "val_value_20": null<br/>
                }<br/>
              ]<br/>
            }<br/>
<br/>
## object_parts/changed [/object_parts/changed/{?token,software_token,opr_timestamp_mutate}]<br/>
<br/>
This api is used to fetch changed object_parts. A change can be made from the app. Use the object_parts to pass a timestamp Y-m-d H:i:s to only show records mutated after that timestamp.<br/>
<br/>
<br/>
### Get changed objects [GET]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [<br/>
                 {<br/>
                    "opr_obj_code": "Object 1",<br/>
                    "opr_prt_code": "001",<br/>
                    "opr_serial_number": "65644456",<br/>
                    "opr_description": "",<br/>
                    "opr_timestamp_installation": "2018-10-11",<br/>
                    "opr_warranty_months": "24",<br/>
                    "opr_timestamp_warranty_expires": "2020-10-11",<br/>
                    "opr_amount": "4",<br/>
                    "val_value_1": "Free field 1 value",<br/>
                    "val_value_2": "Free field 1 value"<br/>
                    "val_value_3": null,<br/>
                    "val_value_4": null,<br/>
                    "val_value_5": null,<br/>
                    "val_value_6": null,<br/>
                    "val_value_7": null,<br/>
                    "val_value_8": null,<br/>
                    "val_value_9": null,<br/>
                    "val_value_10": null,<br/>
                    "val_value_11": null,<br/>
                    "val_value_12": null,<br/>
                    "val_value_13": null,<br/>
                    "val_value_14": null,<br/>
                    "val_value_15": null,<br/>
                    "val_value_16": null,<br/>
                    "val_value_17": null,<br/>
                    "val_value_18": null,<br/>
                    "val_value_19": null,<br/>
                    "val_value_20": null<br/>
                }<br/>
              ]<br/>
            }<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
    + opr_timestamp_mutate (timestamp,optional) ... Timestamp in Y-m-d H:i:s format.  tware.<br/>
<br/>
     <br/>
## PostWorkorders [/PostWorkorders/{?token,software_token}]<br/>
<br/>
This api is used to post one or more workorders to WorkorderApp.  <br/>
<br/>
A workorder can contain the following data:<br/>
<br/>
| Parameter                    | Detail                                                                                                     | Required | Type (size)   |<br/>
|------------------------------|------------------------------------------------------------------------------------------------------------|----------|---------------|<br/>
| WorkorderNo                  | Unique number from ERP/CRM                                                                                 | Yes      | Varchar (255) |<br/>
| ProjectNr                    | Internal Project number                                                                                    | No       | Varchar (255) |<br/>
| ExternProjectNr              | External Project number                                                                                    | No       | Varchar (255) |<br/>
| CustomerName                 | Customer name                                                                                              | Yes      | Varchar (255) |<br/>
| CustomerDebtorNr             | Customer Debtor number                                                                                     | Yes      | Varchar (255) |<br/>
| CustomerStreet               | Customer street                                                                                            | Yes      | Varchar (255) |<br/>
| CustomerStreetNo             | Customer street number                                                                                     | No       | Varchar (255) |<br/>
| CustomerEmail                | Customer Email                                                                                             | No       | Varchar (255) |<br/>
| CustomerZIP                  | Customer zip code                                                                                          | Yes      | Varchar (255) |<br/>
| CustomerCity                 | Customer city                                                                                              | Yes      | Varchar (255) |<br/>
| CustomerContactPerson        | Customer contact person                                                                                    | Yes      | Varchar (255) |<br/>
| CustomerPhone                | Customer phone number                                                                                      | No       | Varchar (255) |<br/>
| CustomerRemark               | Customer remark                                                                                            | No       | Text (64kb)   |<br/>
| CustomerLatitude             | Latitude of work location, used for navigation and to display on maps.                                     | No       | Float(10,6)   |<br/>
| CustomerLongitude            | Longitude of work location, used for navigation and to display on maps.                                    | No       | Float(10,6)   |<br/>
| CustomerNameInvoice          | Invoice customer name                                                                                      | Yes      | Varchar (255) |<br/>
| CustomerDebtorNrInvoice      | Invoice customer debtor number                                                                             | Yes      | Varchar (255) |<br/>
| CustomerStreetInvoice        | Invoice customer street name                                                                               | Yes      | Varchar (255) |<br/>
| CustomerStreetNoInvoice      | Invoice customer street number                                                                             | No       | Varchar (255) |<br/>
| CustomerEmailInvoice         | Invoice customer email                                                                                     | No       | Varchar (255) |<br/>
| CustomerZIPInvoice           | Invoice customer zip code                                                                                  | Yes      | Varchar (255) |<br/>
| CustomerCityInvoice          | Invoice customer city                                                                                      | Yes      | Varchar (255) |<br/>
| CustomerContactPersonInvoice | Invoice customer contact person                                                                            | Yes      | Varchar (255) |<br/>
| CustomerPhoneInvoice         | Invoice customer phone number                                                                              | No       | Varchar (255) |<br/>
| CustomerRemarkInvoice        | Invoice customer remark                                                                                    | No       | Text (64kb)   |<br/>
| TypeOfWork                   | Installatie, Garantie, Levering, Onderhoud, Project, Regie, Reparatie,  Service, Storing, Verkoop, Verhuur | Yes      | Varchar (255) |<br/>
| WorkDescription              | Work description of the workorder. Visible for customer when signing and when receiving the PDF.           | No       | Text (64kb)   |<br/>
| InternalWorkDescription      | Internal work description of the workorder. Only visible for the employee                                  | No       | Text (64kb)   |<br/>
| PaymentMethod                | niet van toepassing, op rekening, contact voldaan, pin betaling, conform offerte                           | Yes      | Varchar (255) |<br/>
| EmployeeNr                   | Employee Number                                                                                            | No       | Varchar (255) |<br/>
| WorkDate                     | Scheduled date for work (d-m-Y)                                                                            | No       | Varchar (255) |<br/>
| WorkTime                     | Scheduled time for work (H:i)                                                                              | No       | Varchar (255) |<br/>
| WorkEndDate                  | Scheduled end date for work (d-m-Y)                                                                        | No       | Varchar (255) |<br/>
| WorkEndTime                  | Scheduled end time for work (H:i)                                                                          | No       | Varchar (255) |<br/>
| WorkDeadline                 | Scheduled deadline for the workorder.                                                                      | No       | Varchar (255) |<br/>
| WorkDuration                 | Duration of the workorder (in minutes). Used to fill WorkEndDate and WorkEndTime based on WorkDate and WorkTime.        | No       | Integer   |<br/>
| WorkStatus                   | Internal work status code. Can be added through status API.                                                | No       | Varchar (255) |<br/>
| PickupPlanning               | Indication if the work order should be added to batch to be picked up. Value should be 0 or 1.             | No       | Integer       |<br/>
| WebPlanning                  | Indication if webplanning is enabled for this order.                                                       | No       | Integer       |<br/>
| CpnCode                      | Contact person code                                                                                        | No       | Varchar (255) |<br/>
| AdrCode                      | Address code                                                                                               | No       | Varchar (255) |<br/>
| ShortWorkDescription         | Short work description. For example 1 line to show in an overview                                          | No       | Varchar (255) |<br/>
| Comment                      | Additional field for the employee to leave their comment                                                   | No       | Varchar (255) |<br/>
| ErrorCode                    | Selected code as added in the errors API                                                                   | No       | Varchar (255) |<br/>
| ErrorMessage                 | Message corresponding to the selected Error, can be changed by the employee                                | No       | Varchar (255) |<br/>
| SolutionCode                 | Selected code as added in the solutions API                                                                | No       | Varchar (255) |<br/>
| SolutionMessage              | Message corresponding to the selected Solution, can be changed by the employee                             | No       | Varchar (255) |<br/>
| PriorityCode                 | Selected code as added in the priorities API                                                               | No       | Varchar (255) |<br/>
| PriorityMessage              | Message corresponding to the selected Priority, can be changed by the employee                             | No       | Varchar (255) |<br/>
| MinimumHours                 | Minimum amount of hours that the customer should sign for. For example: The customer should always sign for 2 hours. If the employee only registers 25 minutes the customer still gets to see 2 hours.                | No       | Decimal (7,2) |<br/>
| RoundingAmount               | Amount of minutes that the total time should be rounded to. For exammple: Your company only works with amounts of 30 minutes. If the user only registers 40 minutes the customer will have to sign for 60 minutes.                | No       | Varchar (255) |<br/>
| Attachments                  | An array containing multiple files. See specification below.                                               | No       | Array         |<br/>
| Materials                    | An array containing material rows. See specification below.                                                | No       | Array         |<br/>
| Workperiods                  | An array containing workperiod rows. See specification below.                                              | No       | Array         |<br/>
| Forms                        | Array of forms. Each row contains Name, Data and ObjectCode                                                | No       | Array         |<br/>
| Employees                    | Array of employee numbers.                                                                                 | No       | Array         |<br/>
| WorkObjects                  | Array of objects codes.                                                                                    | No       | Array         |<br/>
 <br/>
Attachments specification<br/>
<br/>
| Parameter | Detail                                                                                        | Required | Type (size)   |<br/>
|-----------|-----------------------------------------------------------------------------------------------|----------|---------------|<br/>
| File      | URL of the attachment file. This has to be an existing file. The file is saved on our server. | No       | Varchar (255) |<br/>
| Data      | Base64 encoded file data.                                                                     | No       | Base64        |<br/>
| FileName  | Filename of the Base64 encoded data.                                                          | No       | Varchar (255) |<br/>
<br/>
An attachment can be added by providing a valid URL or by providing Base64 encoded data and filename.<br/>
<br/>
<br/>
Material specification<br/>
<br/>
| Parameter     | Detail                                                             | Required | Type          |<br/>
|---------------|--------------------------------------------------------------------|----------|---------------|<br/>
| MaterialCode  | Article number, code or barcode of this material. Example: A786878 | Yes      | Varchar (255) |<br/>
| MaterialNr    | Amount of this material used. Example: 1                           | Yes      | Decimal       |<br/>
| MaterialPrice | Price of this material. Example: 0,00                              | Yes      | Decimal       |<br/>
| MaterialName  | Material name and/or description. Example: Kleinmateriaal          | Yes      | Varchar (255) |<br/>
| MaterialUnit  | Unit of this material. Example: M2                                 | No       | Varchar (255) |<br/>
| MaterialType  | User defined material type                                         | No       | Varchar (255) |<br/>
| MaterialFreeField1  | User defined field 1                                         | No       | Varchar (255) |<br/>
| MaterialFreeField2  | User defined field 2                                         | No       | Varchar (255) |<br/>
| MaterialFreeField3  | User defined field 3                                         | No       | Varchar (255) |<br/>
| MaterialFreeField4  | User defined field 4                                         | No       | Varchar (255) |<br/>
| MaterialFreeField5  | User defined field 5                                         | No       | Varchar (255) |<br/>
 <br/>
 <br/>
<br/>
Workperiod specification<br/>
<br/>
| Parameter     | Detail                                                    | Required  | Type          |<br/>
|---------------|-----------------------------------------------------------|-----------|---------------|<br/>
| WorkDate      | Date specified in d-m-Y                                   | Yes       | Varchar (255) |<br/>
| BeginTime     | Time specified in H:i                                     | Yes       | Varchar (255) |<br/>
| EndTime       | Time specified in H:i                                     | Yes       | Varchar (255) |<br/>
| Break         | Break time in minutes                                     | No        | Int (11)      |<br/>
| TotalTime     | Sum of EndTime - BeginTime - Break formatted in H:i       | Yes       | Varchar (255) |<br/>
| Travel        | Travel distance                                           | No        | Int (11)      |<br/>
| WorkRemark    | Work remark                                               | No        | Text          |<br/>
| HourType      | Hour type code                                            | No        | Varchar (55)  |<br/>
| EmployeeNr    | Employee nunber                                           | No        | Varchar (55)  |<br/>
<br/>
Example array:<br/>
``` json<br/>
"Workperiods": [<br/>
    {<br/>
        "BeginTime": "08:30",<br/>
        "TotalTime": "03:45",<br/>
        "WorkRemark": "",<br/>
        "WorkDate": "26-09-2013",<br/>
        "EndTime": "12:15",<br/>
        "Travel": "1",<br/>
        "EmployeeNr":"11",<br/>
        "HourType":"001"<br/>
    }<br/>
] <br/>
```<br/>
<br/>
<br/>
Forms specification<br/>
<br/>
| Parameter     | Detail                                                                                                                                | Required | Type          |<br/>
|---------------|---------------------------------------------------------------------------------------------------------------------------------------|----------|---------------|<br/>
| Name          | Name of the form. Will be visible to employee and used to search for data.                                                            | Yes      | Varchar (255) |<br/>
| Data          | JSON data of the Form elements. See forms API for description. When this is empty we will use the name to lookup a predefined form.   | No      | Text (64kb)    |<br/>
| ObjectCode    | Object connected to the form. We will search our list of object for the corresponding object.                                         | No      | Varchar (255)  | <br/>
<br/>
### Post workorders [POST]<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
+ Request Correct list of workorders posted. `response` will contain a list of added workorder where each row has the row_id of the added workorder (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
            [<br/>
              {<br/>
                "WorkorderNo": "AB756X",<br/>
                "ProjectNr": "001",<br/>
                "ExternProjectNr": "EX01",<br/>
                "CustomerName": "Yoran van Arragon",<br/>
                "CustomerDebtorNr": "A985785",<br/>
                "CustomerStreet": "Adres",<br/>
                "CustomerStreetNo": "5",<br/>
                "CustomerEmail": "yoran.arragon@provide.nl",<br/>
                "CustomerZIP": "3454de",<br/>
                "CustomerCity": "De Meern",<br/>
                "CustomerContactPerson": "Yoran van Arragon",<br/>
                "CustomerPhone": "0646321418",<br/>
                "CustomerRemark": "Geen opmerking",<br/>
                "CustomerLatitude": null,<br/>
                "CustomerLongitude": null,<br/>
                "CustomerNameInvoice": "John Doe",<br/>
                "CustomerDebtorNrInvoice": "B985785",<br/>
                "CustomerStreetInvoice": "De Dompelaar",<br/>
                "CustomerStreetNoInvoice": "1-D",<br/>
                "CustomerEmailInvoice": "john.doe@example.com",<br/>
                "CustomerZIPInvoice": "3454WJ",<br/>
                "CustomerCityInvoice": "Amsterdam",<br/>
                "CustomerContactPersonInvoice": "John Doe",<br/>
                "CustomerPhoneInvoice": "0611111111",<br/>
                "CustomerRemarkInvoice": "Geen",<br/>
                "TypeOfWork": "Installatie",<br/>
                "WorkDescription": "Verschillende werkzaamheden",<br/>
                "PaymentMethod": "niet van toepassing",<br/>
                "EmployeeNr": "123",<br/>
                "WorkDate": "11-06-2013",<br/>
                "WorkTime": "10:30",<br/>
                "WorkEndDate": "11-06-2013",<br/>
                "WorkEndTime": "12:30",<br/>
                "InternalWorkDescription": "",<br/>
                "WorkDuration": "0",<br/>
                "WorkStatus": "",<br/>
                "WorkDeadline": "",<br/>
                "PickupPlanning": "0",<br/>
                "WebPlanning": "0", <br/>
                "CpnCode": "", <br/>
                "AdrCode": "", <br/>
                "ShortWorkDescription": "",<br/>
                "Comment": "",<br/>
                "ErrorCode": "",<br/>
                "ErrorMessage": "",<br/>
                "SolutionCode": "",<br/>
                "SolutionMessage": "",<br/>
                "MinimumHours": "0.00",<br/>
                "RoundingAmount": "0.00",<br/>
                "Attachments": [<br/>
                    {<br/>
                    "File": "https://www.werkbonapp.nl/uploads/documents/1389703238_test.pdf"<br/>
                    },<br/>
                    {<br/>
                    "File": "https://www.werkbonapp.nl/uploads/documents/201410031416_test.xlsx"<br/>
                    }<br/>
                ],<br/>
                "Materials": [<br/>
                    {<br/>
                        "MaterialCode": "A786878",<br/>
                        "MaterialNr": "1",<br/>
                        "MaterialPrice": "0,00",<br/>
                        "MaterialName": "Kleinmateriaal",<br/>
                        "MaterialUnit": "M2",<br/>
                        "MaterialType": null,<br/>
                        "MaterialFreeField1": null,<br/>
                        "MaterialFreeField2": null,<br/>
                        "MaterialFreeField3": null,<br/>
                        "MaterialFreeField4": null,<br/>
                        "MaterialFreeField5": null<br/>
                    }<br/>
                ]<br/>
              },<br/>
              {<br/>
                "WorkorderNo": "AB756X1",<br/>
                "ProjectNr": "0011",<br/>
                "ExternProjectNr": "EX011",<br/>
                "CustomerName": "Yoran van Arragon1",<br/>
                "CustomerDebtorNr": "A9857851",<br/>
                "CustomerStreet": "Adres1",<br/>
                "CustomerStreetNo": "51",<br/>
                "CustomerEmail": "yoran.arragon@provide.nl1",<br/>
                "CustomerZIP": "3454de1",<br/>
                "CustomerCity": "De Meern1",<br/>
                "CustomerContactPerson": "Yoran van Arragon1",<br/>
                "CustomerPhone": "06463214181",<br/>
                "CustomerRemark": "Geen opmerking1",<br/>
                "CustomerNameInvoice": "John Doe1",<br/>
                "CustomerDebtorNrInvoice": "B9857851",<br/>
                "CustomerStreetInvoice": "De Dompelaar1",<br/>
                "CustomerStreetNoInvoice": "1-D1",<br/>
                "CustomerEmailInvoice": "john.doe@example.com1",<br/>
                "CustomerZIPInvoice": "3454WJ1",<br/>
                "CustomerCityInvoice": "Amsterdam1",<br/>
                "CustomerContactPersonInvoice": "John Doe1",<br/>
                "CustomerPhoneInvoice": "06111111111",<br/>
                "CustomerRemarkInvoice": "Geen1",<br/>
                "TypeOfWork": "Installatie1",<br/>
                "WorkDescription": "Verschillende werkzaamheden1",<br/>
                "PaymentMethod": "niet van toepassing1",<br/>
                "EmployeeNr": "1231",<br/>
                "WorkDate": "11-06-2011",<br/>
                "WorkTime": "10:30",<br/>
                "WorkEndDate": "11-06-2011",<br/>
                "WorkEndTime": "11:30",<br/>
                "InternalWorkDescription": "",<br/>
                "WorkDuration": "0",<br/>
                "WorkStatus": "",<br/>
                "WorkDeadline": "",<br/>
                "PickupPlanning": "0",<br/>
                "WebPlanning": "0", <br/>
                "CpnCode": "", <br/>
                "AdrCode": "", <br/>
                "WorkObjects":[<br/>
                    "OBJ001",<br/>
                    "OBJ002"<br/>
                ],<br/>
                "Employees":[<br/>
                    "1232"<br/>
                ]<br/>
              }<br/>
            ]           <br/>
        <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [<br/>
                {<br/>
                  "workorder_no": "AB756X"<br/>
                  "row_id": 169824,<br/>
                },<br/>
                {<br/>
                  "workorder_no": "AB756X1"<br/>
                  "row_id": 169825,<br/>
                }<br/>
              ]<br/>
            }<br/>
<br/>
<br/>
+ Request Correct workorder posted including Forms (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
            [<br/>
              {<br/>
                "WorkorderNo": "AB756X1",<br/>
                "ProjectNr": "0011",<br/>
                "ExternProjectNr": "EX011",<br/>
                "CustomerName": "Yoran van Arragon1",<br/>
                "CustomerDebtorNr": "A9857851",<br/>
                "CustomerStreet": "Adres1",<br/>
                "CustomerStreetNo": "51",<br/>
                "CustomerEmail": "yoran.arragon@provide.nl1",<br/>
                "CustomerZIP": "3454de1",<br/>
                "CustomerCity": "De Meern1",<br/>
                "CustomerContactPerson": "Yoran van Arragon1",<br/>
                "CustomerPhone": "06463214181",<br/>
                "CustomerRemark": "Geen opmerking1",<br/>
                "CustomerNameInvoice": "John Doe1",<br/>
                "CustomerDebtorNrInvoice": "B9857851",<br/>
                "CustomerStreetInvoice": "De Dompelaar1",<br/>
                "CustomerStreetNoInvoice": "1-D1",<br/>
                "CustomerEmailInvoice": "john.doe@example.com1",<br/>
                "CustomerZIPInvoice": "3454WJ1",<br/>
                "CustomerCityInvoice": "Amsterdam1",<br/>
                "CustomerContactPersonInvoice": "John Doe1",<br/>
                "CustomerPhoneInvoice": "06111111111",<br/>
                "CustomerRemarkInvoice": "Geen1",<br/>
                "TypeOfWork": "Installatie1",<br/>
                "WorkDescription": "Verschillende werkzaamheden1",<br/>
                "PaymentMethod": "niet van toepassing1",<br/>
                "EmployeeNr": "1231",<br/>
                "WorkDate": "11-06-2011",<br/>
                "WorkTime": "10:30",<br/>
                "WorkEndDate": "11-06-2011",<br/>
                "WorkEndTime": "11:30",<br/>
                "InternalWorkDescription": "",<br/>
                "WorkDuration": "0",<br/>
                "WorkStatus": "",<br/>
                "WorkDeadline": "",<br/>
                "PickupPlanning": "0",<br/>
                "WebPlanning": "0", <br/>
                "CpnCode": "", <br/>
                "AdrCode": "", <br/>
                "Forms":[<br/>
                    {<br/>
                        "Name": "Form 1",<br/>
                        "Data": "",<br/>
                        "ObjectCode": ""<br/>
                        <br/>
                    } <br/>
                ] <br/>
              }<br/>
            ]           <br/>
        <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [ <br/>
                {<br/>
                  "workorder_no": "AB756X1"<br/>
                  "row_id": 169825,<br/>
                }<br/>
              ]<br/>
            }<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
            [<br/>
              {<br/>
                "ProjectNr": "0011",<br/>
                "ExternProjectNr": "EX011",<br/>
                "CustomerName": "Yoran van Arragon1",<br/>
                "CustomerDebtorNr": "A9857851",<br/>
                "CustomerStreet": "Adres1", <br/>
                "CustomerEmail": "john.doe@example.com1",<br/>
                "CustomerEmailInvoice": "john.doe@example.com1",<br/>
                "CustomerZIPInvoice": "3454WJ1",<br/>
                "CustomerCityInvoice": "Amsterdam1",<br/>
                "CustomerContactPersonInvoice": "John Doe1",<br/>
                "CustomerPhoneInvoice": "06111111111",<br/>
                "CustomerRemarkInvoice": "Geen1",<br/>
                "TypeOfWork": "Installatie1",<br/>
                "WorkDescription": "Verschillende werkzaamheden1",<br/>
                "PaymentMethod": "niet van toepassing1",<br/>
                "EmployeeNr": "1231",<br/>
                "WorkDate": "11-06-2011",<br/>
                "WorkTime": "10:31"<br/>
              }<br/>
            ]            <br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1501,<br/>
              "messages": [<br/>
                "Required field missing: WorkorderNo",<br/>
                "Required field missing: CustomerZIP",<br/>
                "Required field missing: CustomerCity",<br/>
                "Required field missing: CustomerContactPerson",<br/>
                "Required field missing: CustomerNameInvoice",<br/>
                "Required field missing: CustomerDebtorNrInvoice",<br/>
                "Required field missing: CustomerStreetInvoice",<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
## UpdateWorkorder [/UpdateWorkorder/{?token,software_token,row_id,workorder_no,workdate,worktime,employee_nr,workstatus}]<br/>
<br/>
This API is used to update an existing workorder. The row_id of workorder_no can be used to identify the specific workorder. <br/>
<br/>
### Update an existing workorder [GET]<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
    + row_id (int,required) ... WorkorderApp row id returned when POSTing a workorder<br/>
    + workorder_no (string,required) ... External software workorder number. Added when using the PostWorkorder api<br/>
    + workdate (string,required, `05-03-2016`) ... New workdate for this worksheet. Format : d-m-Y<br/>
    + worktime (string,required,`16:45`) ...  New worktime for this worksheet. Format: H:i<br/>
    + employee_nr (string,required, `67`) ... New employee nr for this worksheet. An employee with this number must exist.<br/>
    + workstatus (string,optional, `001`) ... New workstatus for this worksheet.<br/>
<br/>
+ Request Request with specified parameters having correct values (application/json)<br/>
   <br/>
+ Response 200 (application/json)<br/>
   <br/>
   + Body<br/>
            <br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": null<br/>
            }<br/>
<br/>
<br/>
+ Request Request with parameters having incorrect values (application/json)<br/>
   <br/>
+ Response 200 (application/json)<br/>
   <br/>
   + Body<br/>
            <br/>
            {<br/>
              "code": 1504,<br/>
              "messages": [<br/>
                "Date invalid. Format: 20-02-2016",<br/>
                "Time invalid. Format: 07:08",<br/>
                "Employee not updated"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
            <br/>
+ Request Request with unknown worksheet based on row_id or workorder_no  (application/json)<br/>
   <br/>
+ Response 200 (application/json)<br/>
   <br/>
   + Body<br/>
            <br/>
            {<br/>
              "code": 1500,<br/>
              "messages": [],<br/>
              "response": null<br/>
            }<br/>
## GetWorkorder [/GetWorkorder/{?token,software_token,row_id,workorder_no,update_status}]<br/>
<br/>
This api is used to get a single workorder from WorkorderApp. Either row_id or workorder_no is required as input parameter.<br/>
<br/>
### Get workorder [GET]<br/>
<br/>
<br/>
A workorder contains the following data:<br/>
<br/>
| Parameter                    | Detail                                                                                                    |<br/>
|------------------------------|-----------------------------------------------------------------------------------------------------------|<br/>
| Id                           | WBA database unique row number                                                                            |<br/>
| WorkorderNo                  | Unique number originated from ERP/CRM                                                                     |<br/>
| Order Nr                     | Unique Workorder number created in tablet app                                                             |<br/>
| WorkDate                     | Scheduled date for work (d-m-Y)                                                                      |<br/>
| WorkTime                     | Scheduled time for work (H:i)                                                                           |<br/>
| WorkEndDate                  | Scheduled end date for work (d-m-Y)                                                                  |<br/>
| WorkEndTime                  | Scheduled end time for work (H:i)                                                                       |<br/>
| ProjectNr                    | Internal Project number                                                                                   |<br/>
| ExternProjectNr              | External Project number                                                                                   |<br/>
| CustomerName                 | Customer name                                                                                             |<br/>
| CustomerDebtorNr             | Customer debtor number                                                                                    |<br/>
| CustomerStreet               | Customer street                                                                                           |<br/>
| CustomerStreetNo             | Customer street number                                                                                    |<br/>
| CustomerEmail                | Customer Email                                                                                            |<br/>
| CustomerZIP                  | Customer zip code                                                                                         |<br/>
| CustomerCity                 | Customer city                                                                                             |<br/>
| CustomerContactPerson        | Customer contact person                                                                                   |<br/>
| CustomerPhone                | Customer phone number                                                                                     |<br/>
| CustomerRemark               | Customer remark                                                                                           |<br/>
| CustomerNameInvoice          | Invoice customer name                                                                                     |<br/>
| CustomerDebtorNrInvoice      | Invoice customer debtor number                                                                            |<br/>
| CustomerStreetInvoice        | Invoice customer street name                                                                              |<br/>
| CustomerStreetNoInvoice      | Invoice customer street number                                                                            |<br/>
| CustomerEmailInvoice         | Invoice customer email                                                                                    |<br/>
| CustomerZIPInvoice           | Invoice customer zip code                                                                                 |<br/>
| CustomerCityInvoice          | Invoice customer city                                                                                     |<br/>
| CustomerContactPersonInvoice | Invoice customer contact person                                                                           |<br/>
| CustomerPhoneInvoice         | Invoice customer phone number                                                                             |<br/>
| CustomerRemarkInvoice        | Invoice customer remark                                                                                   |<br/>
| TypeOfWork                   | Installatie, Garantie, Levering, Onderhoud, Project, Regie, Reparatie,Service, Storing, Verkoop, Verhuur  |<br/>
| WorkDescription              | Work description of executed work                                                                         |<br/>
| WorkInstruction              | Work instructions from ERP / CRM (future use)                                                             |<br/>
| PaymentMethod                | niet van toepassing, op rekening, contact voldaan, pin betaling, conform offerte                          |<br/>
| CreationDate                 | Date time of creation of workorder in WBA backoffice                                                      |<br/>
| EmployeeNr                   | Employee Number                                                                                           |<br/>
| Signature                    | Signature file name                                                                                       |<br/>
| SignatureUrl                 | Url to download/open signature image                                                                      |<br/>
| PdfUrl                       | Url to download/open PDF                                                                                  |<br/>
| WordUrl                      | Url to download/open Word document                                                                        |<br/>
| WorksheetCode                | Unique code to use when retrieving a document                                                             |<br/>
| Status                       | Status of the workorder                                                                                   |<br/>
| WorkFinished                 | Indication if the work is finished. When the value is 1 the employee marked the work ready in the tablet. |<br/>
| Archived                     | Indication if the workorder is archived                                                                   |<br/>
| Photos                       | Array of photo objects (URL's)                                                                            |<br/>
| Workperiods                  | Array of Workperiods                                                                                      |<br/>
| Materials                    | Array of used materials (MaterialNr is amount of materials)                                               |<br/>
| Documents                    | Array of file names                                                                                       |<br/>
| Forms                        | Array of forms. Each row contains Name, Data and ObjectCode                                               |<br/>
| Employees                    | Array of employee numbers.                                                                                |<br/>
| WorkObjects                  | Array of objects codes.                                                                                          |<br/>
 <br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
    + row_id (string,required) ... Unique row id received when using the PostWorkorders API <br/>
    + workorder_no (string,required) ... Unique WorkorderNo that was posted in the PostWorkorders API<br/>
    + update_status (boolean, `true`) ... true (default) updates all fetched workorders to status Afgehandeld. false will not update the status.<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body <br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": <br/>
                    {<br/>
                        "id": "1919",<br/>
                        "WorkorderNo": "AB756X",<br/>
                        "OrderNr": "3BCE7228843",<br/>
                        "WorkDate": "11-06-2013",<br/>
                        "WorkTime": "10:30",<br/>
                        "WorkEndDate": "11-06-2013",<br/>
                        "WorkEndTime": "12:30",<br/>
                        "ProjectNr": "001",<br/>
                        "ExternProjectNr": "EX01",<br/>
                        "CustomerName": "Yoran van Arragon",<br/>
                        "CustomerDebtorNr": "A985785",<br/>
                        "CustomerStreet": "Adres",<br/>
                        "CustomerStreetNo": "5",<br/>
                        "CustomerEmail": "yoran.arragon@provide.nl",<br/>
                        "CustomerZIP": "3454de",<br/>
                        "CustomerCity": "De Meern",<br/>
                        "CustomerContactPerson": "Yoran van Arragon",<br/>
                        "CustomerPhone": "0646321418",<br/>
                        "CustomerRemark": "Geen opmerking",<br/>
                        "CustomerNameInvoice": "John Doe",<br/>
                        "CustomerDebtorNrInvoice": "B985785",<br/>
                        "CustomerStreetInvoice": "De Dompelaar",<br/>
                        "CustomerStreetNoInvoice": "1-D",<br/>
                        "CustomerEmailInvoice": "john.doe@example.com",<br/>
                        "CustomerZIPInvoice": "3454WJ",<br/>
                        "CustomerCityInvoice": "Amsterdam",<br/>
                        "CustomerContactPersonInvoice": "John Doe",<br/>
                        "CustomerPhoneInvoice": "0611111111",<br/>
                        "CustomerRemarkInvoice": "Geen",<br/>
                        "TypeOfWork": "Installatie",<br/>
                        "WorkDescription": "Verschillende werkzaamheden",<br/>
                        "PaymentMethod": "niet van toepassing",<br/>
                        "CreationDate": "2013-06-11 02:51",<br/>
                        "Archived": "0",<br/>
                        "EmployeeNr": "",<br/>
                        "Signature": "553b6a0b3ace6c.png",<br/>
                        "SignatureUrl": "http://www.werkbonapp.nl/uploads/handtekeningen/553b6a0b3ace6c.png",<br/>
                        "PdfUrl": "http://www.werkbonapp.nl/mailpdf.php?action=display&sheet_id=6201090a4cf6e501f9f0d7a1c75c584d",<br/>
                        "WordUrl": "http://www.werkbonapp.nl/mailpdf.php?action=word&sheet_id=6201090a4cf6e501f9f0d7a1c75c584d",<br/>
                        "WorksheetCode":"6201090a4cf6e501f9f0d7a1c75c584d",<br/>
                        "status": "Klaargezet",<br/>
                        "WorkFinished": "1",<br/>
                        "InternalWorkDescription": "",<br/>
                        "WorkDuration": "0",<br/>
                        "WorkStatus": "",<br/>
                        "WorkDeadline": "",<br/>
                        "PickupPlanning": "0",<br/>
                        "WebPlanning": "0", <br/>
                        "CpnCode": "", <br/>
                        "AdrCode": "", <br/>
                        "Photos": [<br/>
                            {<br/>
                                "image": "http://www.werkbonapp.nl/werkbonimages/url.png",<br/>
                                "title": "WorkOrderImage_4"<br/>
                            }<br/>
                        ],<br/>
                        "Workperiods": [<br/>
                            {<br/>
                                "BeginTime": "08:30",<br/>
                                "TotalTime": "03:45",<br/>
                                "WorkRemark": "",<br/>
                                "WorkDate": "26-09-2013",<br/>
                                "EndTime": "12:15",<br/>
                                "Travel": "1",<br/>
                                "EmployeeNr":"11",<br/>
                                "HourType":"001"<br/>
                            }<br/>
                        ],<br/>
                        "Materials": [<br/>
                            {<br/>
                                "MaterialCode": "A786878",<br/>
                                "MaterialTotalPrice": "0,00",<br/>
                                "MaterialNr": "1",<br/>
                                "MaterialPrice": "0,00",<br/>
                                "MaterialName": "Kleinmateriaal"<br/>
                                "MaterialUnit": "M2",<br/>
                                "MaterialType": null,<br/>
                                "MaterialFreeField1": null,<br/>
                                "MaterialFreeField2": null,<br/>
                                "MaterialFreeField3": null,<br/>
                                "MaterialFreeField4": null,<br/>
                                "MaterialFreeField5": null<br/>
                            }<br/>
                        ],  <br/>
                        "Documents": [<br/>
                            {<br/>
                            "http://www.werkbonapp.nl/uploads/documents/1389703238_test.pdf",<br/>
                            "http://www.werkbonapp.nl/uploads/documents/201410031416_test.xlsx"<br/>
                            }<br/>
                        ],<br/>
                        "Forms":[],<br/>
                        "WorkObjects":[]<br/>
                    }<br/>
            }<br/>
## GetWorkorders [/GetWorkorders/{?token,software_token,status,update_status,workstatus}]<br/>
<br/>
This api is used to get a list of workorders from WorkorderApp.<br/>
<br/>
### Get workorders [GET]<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
    + status (string, required, `Alle`) ... Status of the workorders that need to be fetched. Possible values: `Alle` , `Opgehaald`, `Klaargezet`, `Compleet` of `Afgehandeld`.<br/>
    + update_status (boolean, `true`) ... true (default) updates all fetched workorders to status Afgehandeld. false will not update the status.<br/>
    + workstatus (string, optional, `001`) ... An extra filter to only receive workorders given a certain workstatus.<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [<br/>
                    {<br/>
                        "id": "1919",<br/>
                        "WorkorderNo": "AB756X",<br/>
                        "OrderNr": "3BCE7228843",<br/>
                        "WorkDate": "11-06-2013",<br/>
                        "WorkTime": "10:30",<br/>
                        "WorkEndDate": "",<br/>
                        "WorkEndTime": "",<br/>
                        "ProjectNr": "001",<br/>
                        "ExternProjectNr": "EX01",<br/>
                        "CustomerName": "Yoran van Arragon",<br/>
                        "CustomerDebtorNr": "A985785",<br/>
                        "CustomerStreet": "Adres",<br/>
                        "CustomerStreetNo": "5",<br/>
                        "CustomerEmail": "yoran.arragon@provide.nl",<br/>
                        "CustomerZIP": "3454de",<br/>
                        "CustomerCity": "De Meern",<br/>
                        "CustomerContactPerson": "Yoran van Arragon",<br/>
                        "CustomerPhone": "0646321418",<br/>
                        "CustomerRemark": "Geen opmerking",<br/>
                        "CustomerNameInvoice": "John Doe",<br/>
                        "CustomerDebtorNrInvoice": "B985785",<br/>
                        "CustomerStreetInvoice": "De Dompelaar",<br/>
                        "CustomerStreetNoInvoice": "1-D",<br/>
                        "CustomerEmailInvoice": "john.doe@example.com",<br/>
                        "CustomerZIPInvoice": "3454WJ",<br/>
                        "CustomerCityInvoice": "Amsterdam",<br/>
                        "CustomerContactPersonInvoice": "John Doe",<br/>
                        "CustomerPhoneInvoice": "0611111111",<br/>
                        "CustomerRemarkInvoice": "Geen",<br/>
                        "TypeOfWork": "Installatie",<br/>
                        "WorkDescription": "Verschillende werkzaamheden",<br/>
                        "PaymentMethod": "niet van toepassing",<br/>
                        "CreationDate": "2013-06-11 02:51",<br/>
                        "EmployeeNr": "",<br/>
                        "Archived": "0",<br/>
                        "Signature": "553b6a0b3ace6c.png",<br/>
                        "SignatureUrl": "http://www.werkbonapp.nl/uploads/handtekeningen/553b6a0b3ace6c.png",<br/>
                        "PdfUrl": "http://www.werkbonapp.nl/mailpdf.php?action=display&sheet_id=6201090a4cf6e501f9f0d7a1c75c584d",<br/>
                        "WordUrl": "http://www.werkbonapp.nl/mailpdf.php?action=word&sheet_id=6201090a4cf6e501f9f0d7a1c75c584d",<br/>
                        "WorksheetCode":"6201090a4cf6e501f9f0d7a1c75c584d",<br/>
                        "status": "Klaargezet",<br/>
                        "WorkFinished": "1",<br/>
                        "InternalWorkDescription": "",<br/>
                        "WorkDuration": "0",<br/>
                        "WorkStatus": "",<br/>
                        "WorkDeadline": "",<br/>
                        "PickupPlanning": "0",<br/>
                        "WebPlanning": "0", <br/>
                        "CpnCode": "", <br/>
                        "AdrCode": "", <br/>
                        "Photos": [<br/>
                            {<br/>
                                "image": "http://www.werkbonapp.nl/werkbonimages/url.png",<br/>
                                "title": "WorkOrderImage_4"<br/>
                            }<br/>
                        ],<br/>
                        "Workperiods": [<br/>
                            {<br/>
                                "BeginTime": "08:30",<br/>
                                "TotalTime": "03:45",<br/>
                                "WorkRemark": "",<br/>
                                "WorkDate": "26-09-2013",<br/>
                                "EndTime": "12:15",<br/>
                                "Travel": "1",<br/>
                                "EmployeeNr":"",<br/>
                                "HourType":""<br/>
                            }<br/>
                        ],<br/>
                        "Materials": [<br/>
                            {<br/>
                                "MaterialCode": "A786878",<br/>
                                "MaterialTotalPrice": "0,00",<br/>
                                "MaterialNr": "1",<br/>
                                "MaterialPrice": "0,00",<br/>
                                "MaterialName": "Kleinmateriaal"<br/>
                                "MaterialUnit": "M2",<br/>
                                "MaterialType": null,<br/>
                                "MaterialFreeField1": null,<br/>
                                "MaterialFreeField2": null,<br/>
                                "MaterialFreeField3": null,<br/>
                                "MaterialFreeField4": null,<br/>
                                "MaterialFreeField5": null<br/>
                            }<br/>
                        ],  <br/>
                        "Documents": [<br/>
                            {<br/>
                            "http://www.werkbonapp.nl/uploads/documents/1389703238_test.pdf",<br/>
                            "http://www.werkbonapp.nl/uploads/documents/201410031416_test.xlsx"<br/>
                            }<br/>
                        ],<br/>
                        "Forms":[],<br/>
                        "WorkObjects":[]<br/>
                    }<br/>
                ]<br/>
            }<br/>
            <br/>
<br/>
            <br/>
## DeleteEntity [/DeleteEntity/{?token,software_token,delete_all,entity,key,value}]<br/>
<br/>
This API is used to delete an entity from WorkorderApp.<br/>
<br/>
Allowed keys for each entity:<br/>
<br/>
| Entity                                  | Key           | Description                                                                               |<br/>
|-----------------------------------------|---------------|-------------------------------------------------------------------------------------------|<br/>
| workorder, employee, material, relation | db_row        | Row id of the entity                                                                      |<br/>
| workorder                               | workorder_no  | External workorder number added when using the PostWorkorders API.                        |<br/>
| workorder                               | order_no      | Order number given in the PostWorkorders API or added by the employee in the application. |<br/>
| employee                                | number        | Employee number added in the when using the employees POST method.                            |<br/>
| material                                | code          | Material code added in the when using the materials POST method.                              |<br/>
| material                                | description   | Material description added in the when using the materials POST method.                       |<br/>
| relation                                | name          | Company/relation name added when using the relations POST method.                             |<br/>
| relation                                | debtor_number | Debtor number added when using the relations POST method.                                |<br/>
| project                                 | code          | Code added when using the projects POST method.                                |<br/>
| hourtype                                | code          | Code added when using the hourtype POST method.                                |<br/>
| category                                | code          | Code added when using the categories POST method.                                |<br/>
| address                                 | code          | Code added when using the addresses POST method.                                |<br/>
| contactperson                           | code          | Code added when using the contactpersons POST method.                                |<br/>
| object                                  | code          | Code added when using the objects POST method.                                |<br/>
| location                                | identifier    | Identifier added when using the locations POST method.                                |<br/>
| material_category                       | mct_mat_code  | Material code added when using the material_categories POST method.                                |<br/>
| material_category                       | mct_cat_code  | Category code added when using the material_categories POST method.                                |<br/>
| error                                   | code          | Code added when using the errors POST method.                                |<br/>
| priority                                | code          | Code added when using the priorities POST method.                                |<br/>
| solution                                | code          | Code added when using the solutions POST method.                                |<br/>
| region                                | code          | Code added when using the regions POST method.                                |<br/>
| vehicle                                | license_plate          | License plate added when using the vehicles POST method.                                |<br/>
| object_part                                | obj_code          | Object code when added with the POST method.                                |<br/>
| object_part                                | prt_code          | Part code when added with the POST method.                                |<br/>
| object_part                                | serial_number          | Serial number when added with the POST method.                                |<br/>
<br/>
Since object_part uses composite primary key it is allowed to add keys and values as an array:<br/>
&delete_all=false&entity=object_part&key[]=prt_code&value[]=0010&key[]=obj_code&value[]=2<br/>
<br/>
### Delete an entity [GET]<br/>
<br/>
object will contain the amount of affected rows.<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
    + delete_all (boolean,required, `false`) ... true or false<br/>
    + entity (string,required, `workorder`) ... workorder, employee, material, relation, project or hourtype<br/>
    + key (string,required, `workorder_no`) ... A key that is allowed for the given entity.<br/>
    + value (string,required,`AB756X`) ...  Value of the given key<br/>
<br/>
+ Request Correct request(application/json) <br/>
<br/>
+ Response 200 (application/json)<br/>
   <br/>
   + Body<br/>
             <br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": 1<br/>
            }<br/>
            <br/>
+ Request Request with wrong entity (application/json) <br/>
<br/>
+ Response 200 (application/json)<br/>
   <br/>
   + Body <br/>
            <br/>
            {<br/>
              "code": 1600,<br/>
              "messages": [<br/>
                "Entity: materials not found"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
<br/>
+ Request Request with wrong key for entity (application/json) <br/>
<br/>
+ Response 200 (application/json)<br/>
   <br/>
   + Body <br/>
            <br/>
            {<br/>
              "code": 1600,<br/>
              "messages": [<br/>
                "Key: codes not allowed for entity: material"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
+ Request Request with delete all true while entity is workorder (application/json) <br/>
<br/>
+ Response 200 (application/json)<br/>
   <br/>
   + Body <br/>
   <br/>
            {<br/>
              "code": 1600,<br/>
              "messages": [<br/>
                "Delete all not allowed on Workorder entity"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
            <br/>
+ Request Request with delete all true while entity is relation (application/json) <br/>
<br/>
+ Response 200 (application/json)<br/>
   <br/>
   + Body<br/>
   <br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": 60<br/>
            }<br/>
<br/>
## locations [/locations/{?token,software_token}]<br/>
<br/>
This api is used to get the locations of connected devices from WorkorderApp or post locations for certain identifiers. An identifier can be anything, for example employee nr or license plate. When posting a location the type should be specified. <br/>
<br/>
Post data should contain an array with objects containing the following parameters:<br/>
<br/>
<br/>
| Parameter                 | Description                                                       | <br/>
|---------------------------|-------------------------------------------------------------------|  <br/>
| lat                       | Latitude                                                          |  <br/>
| long                      | Longitude                                                         |  <br/>
| identifier                | Unique identifier, for example employee number or license plate.  |  <br/>
| type                      | 0 for employee, 1 for car                                         |  <br/>
<br/>
<br/>
### Get location [GET]<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
+ Request Request with location data present.(application/json)<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [<br/>
                {<br/>
                  "customer_id": "1205",<br/>
                  "lat": "50.827024870303866",<br/>
                  "long": "6.018792792566475",<br/>
                  "employee_nr": "123",<br/>
                  "last_seen": "2016-04-06 11:30:00"<br/>
                }<br/>
              ]<br/>
            }<br/>
            <br/>
+ Request Request with no location data present.(application/json)<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body        <br/>
            <br/>
            {<br/>
              "code": 1400,<br/>
              "messages": [],<br/>
              "response": null<br/>
            }<br/>
            <br/>
### Post locations [POST]<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
<br/>
+ Request Locations data posted. `response` will contain the amount of locations updated/inserted into WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [  <br/>
                {  <br/>
                    "lat":"52.1175835",<br/>
                    "long":"5.0364392",<br/>
                    "identifier":"EMP001",<br/>
                    "type":"0"<br/>
                },<br/>
                {  <br/>
                    "lat":"52.1175835",<br/>
                    "long":"5.0364392",<br/>
                    "identifier":"44-FPS-2",<br/>
                    "type":"1"<br/>
                }<br/>
            ]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {"code":200,"messages":[],"response":2}<br/>
<br/>
<br/>
## worktypes [/worktypes/{?token,software_token}]<br/>
<br/>
This api is used to sync  worktypes with WorkorderApp.<br/>
<br/>
Each worktype record can contain the following data:<br/>
<br/>
| Parameter                 | Description                       | Required | Type (size)   |<br/>
|---------------------------|-----------------------------------|----------|---------------|<br/>
| wrt_name                  | Name                              | Y        | Varchar (255) |<br/>
| wrt_description           | Description                       | Y        | Varchar (255) |<br/>
| wrt_default_minutes       | Default minutes used for planning | Y        | Int (10) |<br/>
| wrt_active                | Indicates if worktype is active   | Y        | Int (10)      |<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add worktypes [POST]<br/>
<br/>
<br/>
+ Request Worktypes data posted. `response` will contain the amount of worktypes synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [<br/>
                {<br/>
                  "wrt_name": "Garantie",<br/>
                  "wrt_description": "Garantie werkzaamheden",<br/>
                  "wrt_default_minutes": "60",<br/>
                  "wrt_active": "1"<br/>
                },<br/>
                {<br/>
                  "wrt_name": "Installatie",<br/>
                  "wrt_description": "Installatie werkzaamheden",<br/>
                  "wrt_default_minutes": "720",<br/>
                  "wrt_active": "1"<br/>
                }<br/>
            ] <br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {"code":200,"messages":[],"response":2}<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
        <br/>
            <br/>
            [<br/>
                {<br/>
                  "wrt_description": "Garantie werkzaamheden",<br/>
                  "wrt_default_minutes": "60",<br/>
                  "wrt_active": "1"<br/>
                },<br/>
                {<br/>
                  "wrt_name": "Installatie",<br/>
                  "wrt_description": "Installatie werkzaamheden",<br/>
                  "wrt_default_minutes": "720",<br/>
                  "wrt_active": "1"<br/>
                }<br/>
            ] <br/>
        <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 2601,<br/>
              "messages": [<br/>
                "Required field missing: wrt_name"<br/>
              ],<br/>
              "response": null<br/>
            }  <br/>
            <br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [<br/>
                {<br/>
                  "wrt_name"": "Garantie",<br/>
                  "wrt_description": "Garantie werkzaamheden",<br/>
                  "wrt_default_minutes": "60",<br/>
                  "wrt_active": "1"<br/>
                },<br/>
                {<br/>
                  "wrt_name": "Installatie",<br/>
                  "wrt_description": "Installatie werkzaamheden",<br/>
                  "wrt_default_minutes": "720",<br/>
                  "wrt_active": "1"<br/>
                }<br/>
            ]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1009,"messages":["Unable to parse body"],"response":null}<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1008,<br/>
              "messages": [<br/>
                "Unable to fetch body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
### Get worktypes [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [<br/>
                {<br/>
                  "wrt_name": "Garantie",<br/>
                  "wrt_description": "Garantie werkzaamheden",<br/>
                  "wrt_default_minutes": "60",<br/>
                  "wrt_active": "1"<br/>
                },<br/>
                {<br/>
                  "wrt_name": "Installatie",<br/>
                  "wrt_description": "Installatie werkzaamheden",<br/>
                  "wrt_default_minutes": "720",<br/>
                  "wrt_active": "1"<br/>
                }<br/>
              ]<br/>
            }<br/>
<br/>
<br/>
<br/>
<br/>
## paymentmethods [/paymentmethods/{?token,software_token}]<br/>
<br/>
This api is used to sync paymentmethods with WorkorderApp.<br/>
<br/>
Each paymentmethods record can contain the following data:<br/>
<br/>
| Parameter                 | Description                       | Required | Type (size)   |<br/>
|---------------------------|-----------------------------------|----------|---------------|<br/>
| pmd_description           | Description                       | Y        | Varchar (255) | <br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add paymentmethods [POST]<br/>
<br/>
<br/>
+ Request Paymentmethods data posted. `response` will contain the amount of paymentmethods synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [<br/>
                {<br/>
                  "pmd_description": "Cash"<br/>
                },<br/>
                {<br/>
                  "pmd_description": "Pin"<br/>
                }<br/>
            ]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {"code":200,"messages":[],"response":2}<br/>
    <br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [<br/>
                {<br/>
                  "pmd_description"": "Cash"<br/>
                },<br/>
                {<br/>
                  "pmd_description": "Pin"<br/>
                }<br/>
              ]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1009,"messages":["Unable to parse body"],"response":null}<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1008,<br/>
              "messages": [<br/>
                "Unable to fetch body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
### Get paymentmethods [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [<br/>
                {<br/>
                  "pmd_description": "Cash"<br/>
                },<br/>
                {<br/>
                  "pmd_description": "Pin"<br/>
                }<br/>
              ]<br/>
            }<br/>
<br/>
<br/>
        <br/>
        <br/>
        <br/>
<br/>
## priorities [/priorities/{?token,software_token}]<br/>
<br/>
This api is used to sync priorities with WorkorderApp.<br/>
<br/>
Each priority record can contain the following data:<br/>
<br/>
| Parameter                 | Description                                                                         | Required | Type (size)   |<br/>
|---------------------------|-------------------------------------------------------------------------------------|----------|---------------|<br/>
| code                      | Unique code                                                                         | Y        | Varchar (255) | <br/>
| description               | Description of the priority. The employee can edit this when added to a work order. | Y        | Varchar (255) | <br/>
| app_enabled               | Indication if the priority should be visible in the app                             | N        | Integer (11)  | <br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add priorities [POST]<br/>
<br/>
<br/>
+ Request priorities data posted. `response` will contain the amount of priorities synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"code":"10","description":"High","app_enabled":"0"},{"code":"1","description":"Low","app_enabled":"0"}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {"code":200,"messages":[],"response":2}<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
        <br/>
            <br/>
            [{"code":"10","app_enabled":"0"},{"code":"1","description":"Low","app_enabled":"0"}]<br/>
        <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1051,"messages":["Required field missing: description"],"response":null}<br/>
<br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"code":"10"","app_enabled":"0"},{"code":"1","description":"Low","app_enabled":"0"}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1009,"messages":["Unable to parse body"],"response":null}<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1008,"messages":["Unable to fetch body"],"response":null}<br/>
            <br/>
### Get priorities [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":200,"messages":[],"response":[{"code":"10","description":"High","app_enabled":"0"},{"code":"1","description":"Low","app_enabled":"1"}]}<br/>
            <br/>
<br/>
## errors [/errors/{?token,software_token}]<br/>
<br/>
This api is used to sync errors with WorkorderApp.<br/>
<br/>
Each error record can contain the following data:<br/>
<br/>
| Parameter                 | Description                                                                         | Required | Type (size)   |<br/>
|---------------------------|-------------------------------------------------------------------------------------|----------|---------------|<br/>
| code                      | Unique code                                                                         | Y        | Varchar (255) | <br/>
| description               | Description of the error. The employee can edit this when added to a work order. | Y        | Varchar (255) | <br/>
| app_enabled               | Indication if the error should be visible in the app                             | N        | Integer (11)  | <br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add errors [POST]<br/>
<br/>
<br/>
+ Request errors data posted. `response` will contain the amount of errors synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"code":"GENERAL","description":"General error","app_enabled":"0"},{"code":"MECHANICAL","description":"Mechanical error","app_enabled":"0"},{"code":"SOFTWARE","description":"Software error","app_enabled":"0"}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {"code":200,"messages":[],"response":3}<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
        <br/>
            <br/>
            [{"code":"GENERAL","app_enabled":"0"},{"code":"MECHANICAL","description":"Mechanical error","app_enabled":"0"},{"code":"SOFTWARE","description":"Software error","app_enabled":"0"}]<br/>
        <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1051,"messages":["Required field missing: description"],"response":null}<br/>
<br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"code":"GENERAL"","description":"General error","app_enabled":"0"},{"code":"MECHANICAL","description":"Mechanical error","app_enabled":"0"},{"code":"SOFTWARE","description":"Software error","app_enabled":"0"}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1009,"messages":["Unable to parse body"],"response":null}<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1008,"messages":["Unable to fetch body"],"response":null}<br/>
<br/>
### Get errors [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":200,"messages":[],"response":[{"code":"GENERAL","description":"General error","app_enabled":"0"},{"code":"MECHANICAL","description":"Mechanical error","app_enabled":"0"},{"code":"SOFTWARE","description":"Software error","app_enabled":"0"}]}<br/>
<br/>
## solutions [/solutions/{?token,software_token}]<br/>
<br/>
This api is used to sync solutions with WorkorderApp.<br/>
<br/>
Each solution record can contain the following data:<br/>
<br/>
| Parameter                 | Description                                                                         | Required | Type (size)   |<br/>
|---------------------------|-------------------------------------------------------------------------------------|----------|---------------|<br/>
| code                      | Unique code                                                                         | Y        | Varchar (255) | <br/>
| description               | Description of the solution. The employee can edit this when added to a work order. | Y        | Varchar (255) | <br/>
| app_enabled               | Indication if the solution should be visible in the app                             | N        | Integer (11)  | <br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add solutions [POST]<br/>
<br/>
<br/>
+ Request solutions data posted. `response` will contain the amount of solutions synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"code":"HARD_RESET","description":"Hard reset","app_enabled":"0"},{"code":"SOFT_RESET","description":"Soft reset","app_enabled":"0"},{"code":"Update","description":"Update","app_enabled":"0"}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {"code":200,"messages":[],"response":3}<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
        <br/>
            <br/>
            [{"code":"HARD_RESET","app_enabled":"0"},{"code":"SOFT_RESET","description":"Soft reset","app_enabled":"0"},{"code":"Update","description":"Update","app_enabled":"0"}]<br/>
        <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1051,"messages":["Required field missing: description"],"response":null}<br/>
<br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"code":"HARD_RESET"","description":"Hard reset","app_enabled":"0"},{"code":"SOFT_RESET","description":"Soft reset","app_enabled":"0"},{"code":"Update","description":"Update","app_enabled":"0"}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1009,"messages":["Unable to parse body"],"response":null}<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1008,"messages":["Unable to fetch body"],"response":null}<br/>
<br/>
### Get solutions [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":200,"messages":[],"response":[{"code":"HARD_RESET","description":"Hard reset","app_enabled":"0"},{"code":"SOFT_RESET","description":"Soft reset","app_enabled":"0"},{"code":"Update","description":"Update","app_enabled":"0"}]}<br/>
<br/>
<br/>
## regions [/regions/{?token,software_token}]<br/>
<br/>
This api is used to sync regions with WorkorderApp.<br/>
<br/>
Each region record can contain the following data:<br/>
<br/>
| Parameter                 | Description               | Required | Type (size)   |<br/>
|---------------------------|---------------------------|----------|---------------|<br/>
| reg_code                  | Unique code               | Y        | Varchar (255) | <br/>
| reg_name                  | Name of the region.       | Y        | Varchar (255) | <br/>
| reg_zip_start             | Zip start of the region.  | N        | Integer (11) | <br/>
| reg_zip_end               | Zip end of the region.    | N        | Integer (11) | <br/>
| reg_city                  | City of the region.       | N        | Varchar (255) | <br/>
| reg_country               | Country of the region.    | N        | Varchar (255) | <br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add regions [POST]<br/>
<br/>
<br/>
+ Request solutions data posted. `response` will contain the amount of solutions synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"reg_code":"1","reg_name":"Utrecht 32-33","reg_zip_start":"3200","reg_zip_end":"3500","reg_city":"","reg_country":""},{"reg_code":"2","reg_name":"Utrecht","reg_zip_start":"0","reg_zip_end":"0","reg_city":"Utrecht","reg_country":""}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {"code":200,"messages":[],"response":2}<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
        <br/>
            <br/>
            [{"reg_name":"Utrecht 32-33","reg_zip_start":"3200","reg_zip_end":"3500","reg_city":"","reg_country":""},{"reg_code":"2","reg_name":"Utrecht","reg_zip_start":"0","reg_zip_end":"0","reg_city":"Utrecht","reg_country":""}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1051,"messages":["Required field missing: reg_code"],"response":null}<br/>
<br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"reg_code"":"1","reg_name":"Utrecht 32-33","reg_zip_start":"3200","reg_zip_end":"3500","reg_city":"","reg_country":""},{"reg_code":"2","reg_name":"Utrecht","reg_zip_start":"0","reg_zip_end":"0","reg_city":"Utrecht","reg_country":""}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1009,"messages":["Unable to parse body"],"response":null}<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1008,"messages":["Unable to fetch body"],"response":null}<br/>
<br/>
### Get regions [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":200,"messages":[],"response":[{"reg_code":"1","reg_name":"Utrecht 32-33","reg_zip_start":"3200","reg_zip_end":"3500","reg_city":"","reg_country":""},{"reg_code":"2","reg_name":"Utrecht","reg_zip_start":"0","reg_zip_end":"0","reg_city":"Utrecht","reg_country":""}]}<br/>
            <br/>
            <br/>
## vehicles [/vehicles/{?token,software_token}]<br/>
<br/>
This api is used to sync vehicles with WorkorderApp.<br/>
<br/>
Each vehicle record can contain the following data:<br/>
<br/>
| Parameter                 | Description                                                                         | Required | Type (size)   |<br/>
|---------------------------|-------------------------------------------------------------------------------------|----------|---------------|<br/>
| veh_license_plate         | Unique  license plate                                                                 | Y        | Varchar (255) | <br/>
| veh_title               | Title of the vehicle | Y        | Varchar (255) | <br/>
| veh_brand               | Brand of the vehicle  | N        | Varchar (255) | <br/>
| veh_model               |  Model of the vehicle| N        | Varchar (255) | <br/>
| veh_type               | Type of the vehicle. | N        | Varchar (255) | <br/>
| veh_image               | Url of the image . POST: An external url should be provided.  GET: You will receive a workorderapp url.    | Y        |   | <br/>
| veh_driver               | Driver of the vehicle. This us a reference to the employee number | N        | Varchar (255) | <br/>
| veh_driving               | Indication if the vehicle is driving. When the value is set to 1 it will be shown in the planbord. | N        | Integer (11) | <br/>
| veh_active               | Indication if the vehicle is active                             | N        | Integer (11)  | <br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add vehicles [POST]<br/>
<br/>
<br/>
+ Request solutions data posted. `response` will contain the amount of solutions synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"veh_license_plate":"GN054H","veh_title":"Golf GTE","veh_brand":"Volkswagen","veh_model":"Golf","veh_type":"GTE","veh_driver":"13","veh_driving":"1","veh_active":"1"}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {"code":200,"messages":[],"response":1}<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
        <br/>
            <br/>
            [{"veh_title":"Golf GTE","veh_brand":"Volkswagen","veh_model":"Golf","veh_type":"GTE","veh_driver":"13","veh_driving":"1","veh_active":"1"}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1051,"messages":["Required field missing: veh_license_plate"],"response":null}<br/>
<br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"veh_license_plate":"GN054H","veh_title":"Golf GTE","veh_brand":"Volkswagen","veh_model":"Golf","veh_type":"GTE","veh_driver":"13","veh_driving":"1","veh_active":"1"}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1009,"messages":["Unable to parse body"],"response":null}<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1008,"messages":["Unable to fetch body"],"response":null}<br/>
<br/>
### Get vehicles [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":200,"messages":[],"response":[{"veh_license_plate":"GN054H","veh_title":"Golf GTE","veh_image":"https:\/\/www.wba-werkbonapp.nl\/files\/3bc5037d3987d6710de4c34e7481ca9cb072a61a73cc2e8f6a94e8f16986f1f7\/cfeff9cb262b39015bb079f9845ce917566cf8415bc88a357dfcb5ca120fe738a9a462326ee251764293f4a4e0341d25b665f0f0bd4f128917a7a3454ea574de6e43fc686ba0975cd0b59f0f7d571c194233a4443112f37714e291d607d9bbd8\/cc40a5f5ba28212f2e0ce6336ee211335791ab7126538cb93d954848eb263f14\/51fd23f6accc6e933b732cb5330dfbee3931b23cfc3e258dc10620b28ae03210\/a0631a2843cd949e574754dd9b4b08894b8a031c8856ea08700c051f48ecfa80fade41486bd3b34119c623eab7304aaee1203ace9e669cae2b2aefa232b1192a\/4611bb0557e5077b4f0c0d74ba442f1d52b8a565f6240d9e79e0e804a576b36b8371a6576d1db0517cb93c59f4b96a94f79942bbac94666d61d00ad332b2ff9d\/bf60a587b82325aea37899075b2c03f153ad6f687418c1de3c09ddfcf1ad859f\/1529056261_images.jpg","veh_brand":"Volkswagen","veh_model":"Golf","veh_type":"GTE","veh_driver":"13","veh_driving":"1","veh_active":"1"}]}          <br/>
<br/>
## material_types [/material_types/{?token,software_token}]<br/>
<br/>
This api is used to sync material types with WorkorderApp.<br/>
<br/>
Each material type record can contain the following data:<br/>
<br/>
| Parameter                 | Description                                                                         | Required | Type (size)   |<br/>
|---------------------------|-------------------------------------------------------------------------------------|----------|---------------|<br/>
| code                      | Unique code                                                                         | Y        | Varchar (255) | <br/>
| description               | Description of the material type.  | Y        | Varchar (255) | <br/>
| app_enabled               | Indication if the material type should be visible in the app                             | N        | Integer (11)  | <br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add material_types [POST]<br/>
<br/>
<br/>
+ Request material_types data posted. `response` will contain the amount of material_types synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"code":"DELIVERY","description":"Delivery","app_enabled":"0"},{"code":"ORDER","description":"Order","app_enabled":"0"},{"code":"PICKUP","description":"Pick-up","app_enabled":"0"},{"code":"USAGE","description":"Usage","app_enabled":"0"}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {"code":200,"messages":[],"response":4}<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
        <br/>
            <br/>
            [{"code":"DELIVERY","app_enabled":"0"},{"code":"ORDER","description":"Order","app_enabled":"0"},{"code":"PICKUP","description":"Pick-up","app_enabled":"0"},{"code":"USAGE","description":"Usage","app_enabled":"0"}]<br/>
        <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1051,"messages":["Required field missing: description"],"response":null}<br/>
<br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"code":"DELIVERY"","description":"Delivery","app_enabled":"0"},{"code":"ORDER","description":"Order","app_enabled":"0"},{"code":"PICKUP","description":"Pick-up","app_enabled":"0"},{"code":"USAGE","description":"Usage","app_enabled":"0"}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1009,"messages":["Unable to parse body"],"response":null}<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":1008,"messages":["Unable to fetch body"],"response":null}<br/>
<br/>
### Get material_types [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":200,"messages":[],"response":[{"code":"DELIVERY","description":"Delivery","app_enabled":"0"},{"code":"ORDER","description":"Order","app_enabled":"0"},{"code":"PICKUP","description":"Pick-up","app_enabled":"0"},{"code":"USAGE","description":"Usage","app_enabled":"0"}]}<br/>
                                                <br/>
## workstatusses [/workstatusses/{?token,software_token}]<br/>
<br/>
This api is used to sync workstatusses with WorkorderApp.<br/>
<br/>
Each workstatusses record can contain the following data:<br/>
<br/>
| Parameter                 | Description                       | Required | Type (size)   |<br/>
|---------------------------|-----------------------------------|----------|---------------|<br/>
| sta_code                  | Code                              | Y        | Varchar (255) | <br/>
| sta_name                  | Name                              | Y        | Varchar (255) | <br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add workstatusses [POST]<br/>
<br/>
<br/>
+ Request workstatusses data posted. `response` will contain the amount of statusses synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [<br/>
                {<br/>
                  "sta_code": "002",<br/>
                  "sta_name": "In progress"<br/>
                },<br/>
                {<br/>
                  "sta_code": "001",<br/>
                  "sta_name": "Waiting for customer"<br/>
                }<br/>
            ]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {"code":200,"messages":[],"response":2}<br/>
            <br/>
+ Request Required value missing. (application/json)<br/>
<br/>
    + Body<br/>
        <br/>
            <br/>
            [<br/>
                {<br/>
                  "sta_name": "In progress"<br/>
                },<br/>
                {<br/>
                  "sta_code": "001",<br/>
                  "sta_name": "Waiting for customer"<br/>
                }<br/>
              ]<br/>
        <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 2501,<br/>
              "messages": [<br/>
                "Required field missing: sta_code"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
+ Request Unparsable JSON body posted (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [<br/>
                {<br/>
                  "sta_code"": "002",<br/>
                  "sta_name": "In progress"<br/>
                },<br/>
                {<br/>
                  "sta_code": "001",<br/>
                  "sta_name": "Waiting for customer"<br/>
                }<br/>
            ]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1009,<br/>
              "messages": [<br/>
                "Unable to parse body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
  <br/>
+ Request Empty body posted (application/json)<br/>
<br/>
    + Body<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 1008,<br/>
              "messages": [<br/>
                "Unable to fetch body"<br/>
              ],<br/>
              "response": null<br/>
            }<br/>
<br/>
### Get workstatusses [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response": [<br/>
                {<br/>
                  "sta_code": "002",<br/>
                  "sta_name": "In progress"<br/>
                },<br/>
                {<br/>
                  "sta_code": "001",<br/>
                  "sta_name": "Waiting for customer"<br/>
                }<br/>
              ] <br/>
            }<br/>
            <br/>
            <br/>
## addresses [/addresses/{?token,software_token}]<br/>
<br/>
This api is used to sync addresses with WorkorderApp. An address should always be related to a certain client and can have a main contact person associated with it.<br/>
`adr_code` is used as a unique reference to either insert or update the address. <br/>
<br/>
Each address record can contain the following data:<br/>
<br/>
| Parameter                 | Description                                                                 | Required | Type (size)   |<br/>
|---------------------------|-----------------------------------------------------------------------------|----------|---------------|<br/>
| adr_debtor_nr             | Debtor number of the relation                                               | Y        | Varchar (255) |<br/>
| adr_code                  | Unique code of the address. Used as reference in the workorder.             | Y        | Varchar (255) |<br/>
| adr_cpn_code              | Contact person code of the address                                          | N        | Varchar (255) |<br/>
| adr_line_1                | Address line. Usually street and number.                                    | Y        | Varchar (255) |<br/>
| adr_zip                   | Zipcode of the address                                                      | Y        | Varchar (255) |<br/>
| adr_city                  | City of the adress                                                          | Y        | Varchar (255) |<br/>
| adr_country               | Country of the address                                                      | N        | Varchar (255) |<br/>
| adr_remark                | Remark of the address                                                       | N        | Varchar (255) |<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add addresses [POST]<br/>
<br/>
<br/>
+ Request addresses data posted. `response` will contain the amount of addresses synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [ <br/>
                  { <br/>
                     "adr_debtor_nr":"2082092",<br/>
                     "adr_code":"1",<br/>
                     "adr_cpn_code":"3",<br/>
                     "adr_line_1":"Zonnebaan 9",<br/>
                     "adr_zip":"3542 AA",<br/>
                     "adr_city":"Utrecht",<br/>
                     "adr_country":"Nederland",<br/>
                     "adr_remark":"Crediteurenadministratie"<br/>
                  },<br/>
                  { <br/>
                     "adr_debtor_nr":"82",<br/>
                     "adr_code":"2",<br/>
                     "adr_cpn_code":"3",<br/>
                     "adr_line_1":"Zonnebaan 22",<br/>
                     "adr_zip":"3542 EE",<br/>
                     "adr_city":"Utrecht",<br/>
                     "adr_country":"Nederland",<br/>
                     "adr_remark":""<br/>
                  }<br/>
               ]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {"code":200,"messages":[],"response":2}<br/>
             <br/>
<br/>
### Get addresses [GET]<br/>
<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            { <br/>
               "code":200,<br/>
               "messages":[ <br/>
<br/>
               ],<br/>
               "response":[ <br/>
                  { <br/>
                     "adr_debtor_nr":"2082092",<br/>
                     "adr_code":"1",<br/>
                     "adr_cpn_code":"3",<br/>
                     "adr_line_1":"Zonnebaan 9",<br/>
                     "adr_zip":"3542 AA",<br/>
                     "adr_city":"Utrecht",<br/>
                     "adr_country":"Nederland",<br/>
                     "adr_remark":"Crediteurenadministratie"<br/>
                  },<br/>
                  { <br/>
                     "adr_debtor_nr":"82",<br/>
                     "adr_code":"2",<br/>
                     "adr_cpn_code":"3",<br/>
                     "adr_line_1":"Zonnebaan 22",<br/>
                     "adr_zip":"3542 EE",<br/>
                     "adr_city":"Utrecht",<br/>
                     "adr_country":"Nederland",<br/>
                     "adr_remark":""<br/>
                  }<br/>
               ]<br/>
            }<br/>
<br/>
## address [/address/?token={token}&software_token={software_token}&key={key}&value={value}]<br/>
<br/>
This api is used to fetch addresses based on a filter. <br/>
Filters can be given by adding a key and values array to the URL.<br/>
Adding a single filter: &key=key1&value=value1<br/>
Adding multiple filters: &key[]=key1&value[]=value1&key[]=key2&value[]=value2<br/>
<br/>
### Get objects by filter [GET]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
               "response":[ <br/>
                  { <br/>
                     "adr_debtor_nr":"2082092",<br/>
                     "adr_code":"1",<br/>
                     "adr_cpn_code":"3",<br/>
                     "adr_line_1":"Zonnebaan 9",<br/>
                     "adr_zip":"3542 AA",<br/>
                     "adr_city":"Utrecht",<br/>
                     "adr_country":"Nederland",<br/>
                     "adr_remark":"Crediteurenadministratie"<br/>
                  },<br/>
                  { <br/>
                     "adr_debtor_nr":"82",<br/>
                     "adr_code":"2",<br/>
                     "adr_cpn_code":"3",<br/>
                     "adr_line_1":"Zonnebaan 22",<br/>
                     "adr_zip":"3542 EE",<br/>
                     "adr_city":"Utrecht",<br/>
                     "adr_country":"Nederland",<br/>
                     "adr_remark":""<br/>
                  }<br/>
               ]<br/>
            }<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
    + key (array,optional) ... Filter column, can be any of the allowed parameters.<br/>
    + value (array,optional) ... Filter value.<br/>
<br/>
## contactpersons [/contactpersons/{?token,software_token}]<br/>
<br/>
This api is used to sync contact persons with WorkorderApp. A contact person should always be related to a certain client.<br/>
`cpn_code` is used as a unique reference to either insert or update the address. <br/>
<br/>
Each address record can contain the following data:<br/>
<br/>
| Parameter                 | Description                                                                 | Required | Type (size)   |<br/>
|---------------------------|-----------------------------------------------------------------------------|----------|---------------|<br/>
| cpn_debtor_nr             | Debtor number of the relation                                               | Y        | Varchar (255) |<br/>
| cpn_code                  | Unique code of the contact person. Used as reference in the workorder.      | Y        | Varchar (255) |<br/>
| cpn_name                  | Name of the contact person.                                                 | Y        | Varchar (255) |<br/>
| cpn_phone                 | Phone of the contact person.                                                | N        | Varchar (255) |<br/>
| cpn_email                 | Email of the contact person.                                                | N        | Varchar (255) |<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
<br/>
### Add contact persons [POST]<br/>
<br/>
<br/>
+ Request contact persons data posted. `response` will contain the amount of contact persons synced with WorkOrderApp (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [ <br/>
              { <br/>
                "cpn_debtor_nr":"82",<br/>
                "cpn_code":"1",<br/>
                "cpn_name":"Hans",<br/>
                "cpn_phone":"020 2298144",<br/>
                "cpn_email":"email@email.com"<br/>
              }<br/>
            ]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {"code":200,"messages":[],"response":1}<br/>
             <br/>
### Get contact persons [GET]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            { <br/>
               "code":200,<br/>
               "messages":[ <br/>
    <br/>
               ],<br/>
               "response":[ <br/>
                  { <br/>
                    "cpn_debtor_nr":"82",<br/>
                    "cpn_code":"1",<br/>
                    "cpn_name":"Hans",<br/>
                    "cpn_phone":"020 2298144",<br/>
                    "cpn_email":"email@email.com"<br/>
                  }<br/>
               ]<br/>
            }<br/>
<br/>
## contactperson [/contactperson/?token={token}&software_token={software_token}&key={key}&value={value}]<br/>
<br/>
This api is used to fetch contactpersons based on a filter. <br/>
Filters can be given by adding a key and values array to the URL.<br/>
Adding a single filter: &key=key1&value=value1<br/>
Adding multiple filters: &key[]=key1&value[]=value1&key[]=key2&value[]=value2<br/>
<br/>
### Get objects by filter [GET]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {<br/>
              "code": 200,<br/>
              "messages": [],<br/>
              "response":[ <br/>
                  { <br/>
                    "cpn_debtor_nr":"82",<br/>
                    "cpn_code":"1",<br/>
                    "cpn_name":"Hans",<br/>
                    "cpn_phone":"020 2298144",<br/>
                    "cpn_email":"email@email.com"<br/>
                  }<br/>
               ]<br/>
            }<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
    + key (array,optional) ... Filter column, can be any of the allowed parameters.<br/>
    + value (array,optional) ... Filter value.<br/>
<br/>
<br/>
          <br/>
## invoices [/invoices/?token={token}&software_token={software_token}&key={key}&value={value}&operator={operator}]<br/>
<br/>
This api is used to fetch generated invoices from WorkorderApp.  <br/>
<br/>
The result can be filtered by using the advanced filter. As described in the introduction section.<br/>
<br/>
| Parameter                 | Description                                                                                           |<br/>
|---------------------------|-------------------------------------------------------------------------------------------------------|<br/>
| inv_id                    | Unique invoice ID  number of the invoice                                                              |<br/>
| inv_worksheet_id          | Worksheet ID that is used to generate this invoice                                                    |<br/>
| inv_quo_id                | Quotation ID that is used to generate this invoice                                                    |<br/>
| inv_inv_id                | Parent invoice ID. Used when creating a credit invoice.                                               |<br/>
| inv_type                  | Invoice type, can be DEBIT, CREDIT, CONCEPT_DEBIT or CONCEPT_CREDIT                                   |<br/>
| inv_currency_code         | ISO 4217 currency code                                                                                |<br/>
| inv_currency_symbol       | Currency symbol shown in the UI                                                                       |<br/>
| inv_description           | Description of the invoice                                                                            |<br/>
| inv_invoice_debtor_nr     | Debtor number of the assigned relation                                                                |<br/>
| inv_invoice_debtor_name   | Debtor name of the assigned relation                                                                  |<br/>
| inv_invoice_debtor_email  | Debtor e-mail of the assigned relation                                                                |<br/>
| inv_number_numeric        | Invoice number numeric value                                                                          |<br/>
| inv_number_formatted      | Pretty formatted invoice number                                                                       |<br/>
| inv_status                | Invoice status, can be OPEN, PAYED, OVERDUE, REMINDER_1, REMINDER_2, REMINDER_3 or ...                |<br/>
| inv_reference             | Reference, example purchase order number workorder number                                             |<br/>
| inv_date                  | Invoice date                                                                                          |<br/>
| inv_due_date              | Invoice due date                                                                                      |<br/>
| inv_due_days              | Amount of due days. This days are added to the inv_date to calculate the inv_due_date.                |<br/>
| inv_terms                 | Terms shown in the footer of the PDF.                                                                 |<br/>
| inv_header                | Header shown on top of the PDF.                                                                       |<br/>
| inv_amount                | Total amount including VAT.                                                                           |<br/>
| inv_amount_excl           | Total amount excluding VAT.                                                                           |<br/>
| inv_balance               | Total amounts of the transactions registered to this invoice.                                         |<br/>
| inv_user_create           | User who created this invoice                                                                         |<br/>
| inv_user_mutate           | User who mutated this invoice                                                                         |<br/>
| inv_user_send             | User who marked this invoice as send.                                                                 |<br/>
| inv_timestamp_create      | Timestamp of creation                                                                                 |<br/>
| inv_timestamp_mutate      | Timestamp of mutating                                                                                 |<br/>
| inv_timestamp_payed       | Timestamp when the invoice was marked as payed (inv_amount equal to inv_balance)                      |<br/>
| inv_timestamp_send        | Timestamp of marking the invoice as send.                                                             |<br/>
| iln_lines                 | Array of invoice lines.                                                                               |<br/>
| invoice_debtor            | Invoice debtor.                                                                                       |<br/>
| pdf                       | Temporary PDF url.                                                                                    |<br/>
| ubl                       | Temporary ubl 2.0 url.                                                                                |<br/>
    <br/>
<br/>
Invoice line parameters<br/>
<br/>
| Parameter             | Description                                      |<br/>
|-----------------------|--------------------------------------------------|<br/>
| iln_id                | Line ID                                          |<br/>
| iln_inv_id            | Invoice Id                                       |<br/>
| iln_order             | Position of the line                             |<br/>
| iln_material_code     | Material code                                    |<br/>
| iln_material_hourtype | Hourtype code                                    |<br/>
| iln_description       | Line description                                 |<br/>
| iln_amount            | Line amount                                      |<br/>
| iln_price             | Item price                                       |<br/>
| iln_vat_percentage    | Vat percentage                                   |<br/>
| iln_discount          | Discount percentage                              |<br/>
| iln_total             | Total price excluding vat and discount           |<br/>
| iln_total_discount    | Calculated discount amount                       |<br/>
| iln_total_vat         | Calculated vat amount                            |<br/>
| iln_total_excl        | Total price excluding vat and including discount |<br/>
| iln_total_incl        | Total price including vat and including discount |<br/>
<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
    + key (string, optional, `inv_number_formatted`) ... Key that is matched to the value by the operator<br/>
    + value (integer, optional, `2018-00005`) ... value that is matched to the key by the operator <br/>
    + operator (string, optional, `gt`) ... Operator used to compare the value the key <br/>
    <br/>
### Get invoice [GET]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":200,"messages":[],"response":[{"inv_id":"164","inv_worksheet_id":null,"inv_quo_id":null,"inv_inv_id":null,"inv_type":"DEBIT","inv_currency_code":"EUR","inv_currency_symbol":"\u20ac","inv_description":"","inv_invoice_debtor_nr":"1010101010228","inv_invoice_debtor_name":"van Arragon Bouw","inv_invoice_debtor_email":"yoran122@hotmail.com","inv_number_numeric":"1","inv_number_formatted":"2018-00001","inv_status":"REMINDER_1","inv_reference":"","inv_date":"2018-07-31","inv_due_date":"2018-08-14","inv_due_days":"14","inv_terms":"<p>We verzoeken u vriendelijk het bovenstaande bedrag voor 2018-08-14 te voldoen op onze bankrekening onder vermelding van het factuurnummer 2018-00001.<\/p>\r\n","inv_header":"<p>PTS<br \/>\r\nMandenmakerslaan 58<br \/>\r\n3454DE, De meern<br \/>\r\nNederland<br \/>\r\nKvk: 4243234478<br \/>\r\nBtw: NL012356278.b01<\/p>\r\n","inv_amount":"43.56","inv_amount_excl":"36.00","inv_balance":"0.00","inv_user_create":"Provide","inv_user_mutate":"","inv_user_send":"Provide","inv_timestamp_create":"2018-07-31 07:49:44","inv_timestamp_mutate":null,"inv_timestamp_payed":null,"inv_timestamp_send":"2018-07-31 07:49:56","iln_lines":[{"iln_id":"1883","iln_inv_id":"164","iln_order":"0","iln_material_code":"00000001","iln_material_hourtype":null,"iln_description":"test kostenplaats","iln_amount":"2.00","iln_price":"20.00","iln_vat_percentage":"21.00","iln_discount":"10.00","iln_total":"40.00","iln_total_discount":"4.00","iln_total_vat":"7.56","iln_total_excl":"36.00","iln_total_incl":"43.56"}],"invoice_debtor":{"ind_name":"van Arragon Bouw","ind_debiteur_number":"1010101010228","ind_street":"Amerikalaan 639","ind_zip":"3526VZ","ind_city":"Utrecht","ind_country":"","ind_contact":"yoran van ar","ind_phone":"0646321418","ind_email":"yoran122@hotmail.com"},"pdf":"https:\/\/www.wba-werkbonapp.nl\/files\/2ba6c8fd4294926531464e1b73ada1856ffb659bc6904fd7bff9e4932eaece0c\/36c5b230e0ff666199f8fbd0b9e1d5be505da32f70520c2dfcb0a06ade001908db7c1d0900c9fb01bed3e0e6354f5aeb4b1ecfa573ce5c6f7b476ebd12e024bc0efd2e450df745ce3118d0413340522c86ad5acfca017e61a7ed31a69b2cf9ee\/72ae615104118cbf6549d19046cdc56c65a5a42f10edd21e914cd95394d2d594\/608a7ba4894f913f1a218122617194c7f700b19238ff1e23b435aebeaabe977d\/92ad26aa8ff0f6c286a2f69e7b4d48ced1bc599b6eef2fe14dbb1cd8743ad3f0688610e69788f4e7c823713a0abfeeebb69d6383442fc934544512bba5e6bdeb\/7431a2d509c15d3cebd10ef377f9bde83f1640cf8b5129615c61bbbcb07d5757\/272cf7f4892038a4c839d737a63e19ba814b2a649d443e36031eead31e0942bc4d3ee859b1d802210696c7e9db4e8882b1c79aaa4eea87b81d9cd83d90d5888ed6bbc11f432763e9e3bfd6ab350d6a6257830e2d3e9e8fae50317f363830d0c18afc2448eb4d24d9fa753f39effa2701058892d0191b6ac4aa1c5a68f40a9c44eefe275eb378df6a45c7262898879444c6daaacc0f27984ce62a2b552fd04910d0206a977590eca758e035562905f91efe4cc456ac5232dce0d0e31d9c4521292ea486307c50eb4e2d2510df8b5a1b7e41cd584aa3c710024ef1faf6b4d4c78fad5aaa098a03f7b0dfe4d27f18167f7e24ffd9055f6f26aa2bd7518b74946dbc\/invoicepdf.php","ubl":"https:\/\/www.wba-werkbonapp.nl\/files\/f059865c12c1c91bc0bd2fba97d622502076304c9a7cbb322638f96b52aa3e89\/570bf48bebda4a3881a08a020c74793cc924ccdcbe62d6bdd5024bb765517490db7c1d0900c9fb01bed3e0e6354f5aeb4b1ecfa573ce5c6f7b476ebd12e024bc0efd2e450df745ce3118d0413340522c86ad5acfca017e61a7ed31a69b2cf9ee\/b9cbbbd12b330a8e7dd7d46c1513a2671ccee2d2c0716cf953e2e6751d28e8e5\/605fee22609e1a401e420d9cc0707a925930e24cf5f06e19b82ae4372af36e32\/60c21fd4c1b746ec723f513373bf61121936d3642b8ab7ea3566487db874d8db688610e69788f4e7c823713a0abfeeebb69d6383442fc934544512bba5e6bdeb\/6e4f99f1dd601ad5b1e27234105dd2d6fbcce86d70a188968b87685813516f37\/0dc9bf292d736d2d2a5e22a8c1e92b52538579e38ca0ce8f1d260d06e96750ba4d3ee859b1d802210696c7e9db4e8882b1c79aaa4eea87b81d9cd83d90d5888e80fbda037c5eeb269a3dfb68c2d51f778e9bea26e746bd6e48f82ecc5d14b1dfc3e0c512b2036a02115e1f96a68ec47f45dcaec870fdbcaad0ba540db0cd8cf8e15fec4d19b194bd220c523a9f7524a4a4e8e3c5133b07d80f822c8aac04dea2bffff201bfea5a480474f5a393f166d16e1c8ae033f285503d45b1a24acedd90b6dbf0eb15c3ed460b2fc9f98865707939e90ed8ff8511d7978930d7b21b147e\/invoicepdf.php"}]}<br/>
                 <br/>
## transactions [/transactions/?token={token}&software_token={software_token}&key={key}&value={value}&value={value}&operator={operator}44]<br/>
<br/>
This api is used to fetch a single generated invoice from WorkorderApp.  <br/>
<br/>
Filters can be given by adding a key and values array to the URL.<br/>
Adding a single filter: &key=key1&value=value1&operator=gt<br/>
Adding multiple filters: &key[]=key1&value[]=value1&operator[]=eq&key[]=key2&value[]=value2&operator[]=gt<br/>
<br/>
Following operators are allowed:<br/>
| Operator | Description                 |<br/>
|----------|-----------------------------|<br/>
| li       | Like (%)                    |<br/>
| eq       | Equal (=)                   |<br/>
| ne       | Not equal (!=)              |<br/>
| gt       | Greather than (>)           |<br/>
| ge       | Greather than or equal (>=) |<br/>
| lt       | Less than  (<)              |<br/>
| le       | Less than or equal (<=)     |<br/>
 <br/>
<br/>
Transaction parameters. The invoice id of a transaction transaction can be empty if a transaction is not assigned to an invoice. Once it is assigned the balance of the invoice will be adjusted.<br/>
<br/>
| Paramter                    | Description                                | Type         |<br/>
|-----------------------------|--------------------------------------------|--------------|<br/>
| int_inv_id                  | Invoice ID                                 | int(11)      |<br/>
| int_transaction_id          | Transaction ID                             | varchar(255) |<br/>
| int_external_transaction_id | External Transaction ID                    | varchar(255) |<br/>
| int_description             | Transaction Description                    | varchar(255) |<br/>
| int_amount                  | Transaction amount                         | decimal(7,2) |<br/>
| int_type                    | Transaction type                           | varchar(255) |<br/>
| int_type_description        | Transaction type description               | varchar(255) |<br/>
| int_status                  | Transaction status,NEW or PROCESSED        | varchar(55)  |<br/>
| int_user                    | User/entity who registered the transaction | varchar(255) |<br/>
| int_timestamp               | Timestamp registered                       | timestamp    |<br/>
<br/>
<br/>
+ Parameters<br/>
    + token (string,required ,`0f24d1e07c8609c0fb111fbcc168f9aaa`) ... WorkorderApp customer token<br/>
    + software_token (string,required , `c316c4532fa7cccdcd572491d9552f80945a51366`) ... WorkorderApp external software token<br/>
    + key (string, optional, `int_transaction_id`) ... Key that is matched to the value by the operator<br/>
    + value (integer, optional, `0000009CSD572CE75E21119`) ... value that is matched to the key by the operator <br/>
    + operator (string, optional, `eq`) ... Operator used to compare the value the key <br/>
    <br/>
### Get transactions [GET]<br/>
<br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
<br/>
            {"code":200,"messages":[],"response":[{"int_inv_id":null,"int_transaction_id":"0000009CSD572CE75E21119","int_external_transaction_id":"RABO1212348797128314512435","int_description":"Bank transaction","int_amount":"100.43","int_type":"BANK","int_type_description":"","int_user":"Fremke","int_timestamp":"2018-07-31 11:33:45"},{"int_inv_id":"164","int_transaction_id":"0000009B601572CE75E21111","int_external_transaction_id":"","int_description":"Cash transaction","int_amount":"50.00","int_type":"CASH","int_type_description":"","int_user":"Femke","int_timestamp":"2018-07-31 13:22:38"},{"int_inv_id":"164","int_transaction_id":"0000005B601172CE75E21418","int_external_transaction_id":"IZETTLE5415642351431123231","int_description":"iZettle payment","int_amount":"121.00","int_type":"iZettle","int_type_description":"","int_user":"Femke","int_timestamp":"2018-07-31 09:36:18"}]}<br/>
            <br/>
     <br/>
### Add transactions [POST]<br/>
<br/>
<br/>
+ Request Transaction data posted. (application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"int_inv_id":null,"int_transaction_id":"0000009CSD572CE75E21119","int_external_transaction_id":"RABO1212348797128314512435","int_description":"Bank transaction","int_amount":"100.43","int_type":"BANK","int_type_description":"","int_user":"Fremke","int_timestamp":"2018-07-31 11:33:45"},{"int_inv_id":"164","int_transaction_id":"0000009B601572CE75E21111","int_external_transaction_id":"","int_description":"Cash transaction","int_amount":"50.00","int_type":"CASH","int_type_description":"","int_user":"Femke","int_timestamp":"2018-07-31 13:22:38"},{"int_inv_id":"164","int_transaction_id":"0000005B601172CE75E21418","int_external_transaction_id":"IZETTLE5415642351431123231","int_description":"iZettle payment","int_amount":"121.00","int_type":"iZettle","int_type_description":"","int_user":"Femke"}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {<br/>
                "code": 200,<br/>
                "messages": [],<br/>
                "response": [<br/>
                    {<br/>
                        "int_inv_id": null,<br/>
                        "int_transaction_id": "0000005B6962EBA840119",<br/>
                        "int_external_transaction_id": "RABO1212348797128314512435",<br/>
                        "int_description": "Bank transaction",<br/>
                        "int_amount": "100.43",<br/>
                        "int_type": "BANK",<br/>
                        "int_type_description": "",<br/>
                        "int_status": "PROCESSED",<br/>
                        "int_user": "OpenAPI",<br/>
                        "int_timestamp": "2018-07-31 11:33:45"<br/>
                    },<br/>
                    {<br/>
                        "int_inv_id": "164",<br/>
                        "int_transaction_id": "0000005B6962EBA8BD116419",<br/>
                        "int_external_transaction_id": "",<br/>
                        "int_description": "Cash transaction",<br/>
                        "int_amount": "50.00",<br/>
                        "int_type": "CASH",<br/>
                        "int_type_description": "",<br/>
                        "int_status": "PROCESSED",<br/>
                        "int_user": "OpenAPI",<br/>
                        "int_timestamp": "2018-07-31 13:22:38"<br/>
                    },<br/>
                    {<br/>
                        "int_inv_id": "164",<br/>
                        "int_transaction_id": "0000005B6962EBA9B7116419",<br/>
                        "int_external_transaction_id": "IZETTLE5415642351431123231",<br/>
                        "int_description": "iZettle payment",<br/>
                        "int_amount": "121.00",<br/>
                        "int_type": "iZettle",<br/>
                        "int_type_description": "",<br/>
                        "int_status": "PROCESSED",<br/>
                        "int_user": "OpenAPI",<br/>
                        "int_timestamp": "2018-08-07 11:14:19"<br/>
                    }<br/>
                ]<br/>
            }<br/>
            <br/>
            <br/>
### Update transactions [PUT]<br/>
<br/>
+ Request Transaction data posted. `response` will contain the amount of transactions affected. The request should contain int_transaction_id or int_external_transaction_id as a reference to update.(application/json)<br/>
<br/>
    + Body<br/>
    <br/>
            [{"int_transaction_id":"0000009CSD572CE75E21119","int_inv_id":"164"},{"int_external_transaction_id":"IZETTLE5415642351431123231","int_inv_id":null}]<br/>
            <br/>
+ Response 200 (application/json)<br/>
 <br/>
    + Body<br/>
    <br/>
            {"code":200,"messages":[],"response":2}<br/>

## Authorization

This API does not require authorization.

## Actions

### Add employees
> This api is used to get or edit employees in WorkorderApp.<br/>
> Each employee record can contain the following data:<br/>
> <br/>
> | Parameter  | Required | Type (size)   |<br/>
> |------------|----------|---------------|<br/>
> | firstname  | Y        | Varchar (255) |<br/>
> | lastname   | Y        | Varchar (255) |<br/>
> | number     | Y        | Varchar (255) |<br/>

*Tags:* `Employees`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add projects
> This api is used to sync external projects with WorkorderApp.<br/>
> Each project record can contain the following data:<br/>
> <br/>
> | Parameter        | Required | Type (size)     |<br/>
> |------------------|----------|-----------------|<br/>
> | code             | Y        | Varchar (255)   |<br/>
> | code_ext         | N        | Varchar (255)   |<br/>
> | debtor_number    | Y        | Varchar (255)   |<br/>
> | status           | Y        | Varchar (255)   |<br/>
> | name             | Y        | Varchar (255)   |<br/>
> | description      | N        | Text            |<br/>
> | progress         | N        | Integer         |<br/>
> | date_start       | Y        | Varchar (255)   |<br/>
> | date_end         | N        | Varchar (255)   |<br/>
> | active           | N        | Integer (1 or 0)|<br/>

*Tags:* `Projects`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add projects
> This api is used to sync external projects with WorkorderApp.<br/>
> Each project record can contain the following data:<br/>
> <br/>
> | Parameter        | Required | Type (size)     |<br/>
> |------------------|----------|-----------------|<br/>
> | code             | Y        | Varchar (255)   |<br/>
> | code_ext         | N        | Varchar (255)   |<br/>
> | debtor_number    | Y        | Varchar (255)   |<br/>
> | status           | Y        | Varchar (255)   |<br/>
> | name             | Y        | Varchar (255)   |<br/>
> | description      | N        | Text            |<br/>
> | progress         | N        | Integer         |<br/>
> | date_start       | Y        | Varchar (255)   |<br/>
> | date_end         | N        | Varchar (255)   |<br/>
> | active           | N        | Integer (1 or 0)|<br/>

*Tags:* `Projects activities`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add tasks
> This api is used to sync tasks with OutSmart.<br/>
> Each task record can contain the following data:<br/>
> <br/>
> | Parameter               | Required | Description                                                |<br/>
> |-------------------------|----------|------------------------------------------------------------|<br/>
> | tsk_tsk_id              | N        | Parent tasks ID                                            |<br/>
> | tsk_type                | Y        | Type should be `TASK`                                      |<br/>
> | tsk_name                | Y        | Name description of the task                               |<br/>
> | tsk_description         | N        | Long description, can contain HTML format                  |<br/>
> | tsk_reference           | Y        | External reference used to update same task in the future  |<br/>
> | tsk_category            | Y        | Category used to group in OutSmart in general CALL or MAIL |<br/>
> | tsk_icon                | N        | Icon used phone-square and envelope-o                      |<br/>
> | tsk_owner               | N        | Employee number of the owner                               |<br/>
> | tsk_assigned_to         | N        | Employee number of the assignee                            |<br/>
> | tsk_priority            | Y        | LOW, NORMAL, HIGH                                          |<br/>
> | tsk_status              | Y        | YET_TO_START,IN_PROGRESS,COMPLETED,EXPIRED,CLOSED          |<br/>
> | tsk_debtor_nr           | N        | Connected customer debtor number                           |<br/>
> | tsk_address_nr          | N        | Connected address code                                     |<br/>
> | tsk_contact_nr          | N        | Connected contactperson code                               |<br/>
> | tsk_timestamp_due       | N        | Timestamp due                                              |<br/>
> | tsk_timestamp_create    | N        | Timestamp created                                          |<br/>
> | tsk_timestamp_mutate    | N        | Timestamp mutated                                          |<br/>
> | tsk_timestamp_started   | N        | Timestamp started                                          |<br/>
> | tsk_timestamp_completed | N        | Timestamp completed                                        |<br/>
> | tsk_timestamp_start     | N        | Timestamp start                                            |<br/>
> | tsk_link                | N        | Link(href) to be rendered in the UI                        |<br/>
> | tsk_project_nr          | N        | Connected project number                                   |<br/>
> | tsk_project_activity_nr | N        | Connected project activity number                          |<br/>
> | tsk_order_nr            | N        | Connected work order number                                |<br/>
> | tsk_invoice_number      | N        | Connected invoice number                                   |<br/>
> | tsk_quotation_number    | N        | Connected quotation number                                 |<br/>

*Tags:* `Tasks`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add categories
> This api is used to categories with WorkorderApp.<br/>
> Each category record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                                   | Required | Type (size)   |<br/>
> |---------------------------|-----------------------------------------------|----------|---------------|<br/>
> | cat_code                  | Category code                                 | Y        | Varchar (255) |<br/>
> | cat_cat_code              | Parent category code part                     | N        | Varchar (255) |<br/>
> | cat_name                  | Category name                                 | Y        | Varchar (255) |<br/>
> | cat_image                 | Url of the image. POST: An external url should be provided.  GET: You will receive a workorderapp url.     | N        | Varchar (255)      |<br/>
> | cat_display               | Indication if the category should be displayed| Y        | Int (10)      |<br/>

*Tags:* `Categories`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add hourtypes
> This api is used to sync external hourtypes with WorkorderApp.<br/>
> Each hourtype record can contain the following data:<br/>
> <br/>
> | Parameter        | Required | Type (size)         |<br/>
> |------------------|----------|---------------------|<br/>
> | code             | Y        | Varchar (255)       |<br/>
> | name             | Y        | Varchar (255)       |<br/>
> | cost_booking     | Y        | Integer (1 or 0)    |<br/>
> | sale_booking     | Y        | Integer (1 or 0)    |<br/>
> | sale_price       | Y        | Decimal (> 0)       |<br/>
> | cost_price       | N        | Decimal (> 0)       | <br/>
> | active           | N        | Integer (1 or 0)    |<br/>

*Tags:* `Hourtypes`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add material categories
> This api is used to sync material categories with WorkorderApp.<br/>
> Each material_categories record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                                   | Required | Type (size)   |<br/>
> |---------------------------|-----------------------------------------------|----------|---------------|<br/>
> | mct_mat_code              | Material code                                 | Y        | Varchar (255) |<br/>
> | mct_cat_code              | Category code                                 | Y        | Varchar (255) |<br/>

*Tags:* `Material categories`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add relations
> This api is used to sync external contacts with WorkorderApp.<br/>
> Each relation record can contain the following data:<br/>
> <br/>
> | Parameter        | Required | Type (size)   |<br/>
> |------------------|----------|---------------|<br/>
> | name             | Y        | Varchar (255) |<br/>
> | debtor_number    | Y        | Varchar (255) |<br/>
> | contact          | N        | Varchar (255) |<br/>
> | phone_number     | N        | Varchar (255) |<br/>
> | email            | N        | Varchar (255) |<br/>
> | email_workorder  | N        | Varchar (255) |<br/>
> | street           | Y        | Varchar (255) |<br/>
> | house_number     | N        | Varchar (255) |<br/>
> | postal_code      | Y        | Varchar (255) |<br/>
> | city             | Y        | Varchar (255) |<br/>
> | remark           | N        | Text (64kb)   |<br/>
> | latitude         | N        | Float (10,6)  |<br/>
> | longitude        | N        | Float (10,6)  |<br/>

*Tags:* `Relations`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `test` - _required_
* `Accept` - _required_

### Add materials
> This api is used to sync materials with WorkorderApp.<br/>
> Each material record can contain the following data:<br/>
> <br/>
> | Parameter    | Required | Type (size)   |<br/>
> |--------------|----------|---------------|<br/>
> | code         | Y        | Varchar (255) |<br/>
> | description  | Y        | Text (64kb)   |<br/>
> | price        | Y        | Decimal       |<br/>
> | unit         | Y        | Varchar (255) |<br/>
> | eancode      | N        | Varchar (55)  |<br/>
> | barcode      | N        | Varchar (55)  |<br/>
> | freefield1   | N        | Varchar (255) |<br/>
> | freefield2   | N        | Varchar (255) |<br/>
> | freefield3   | N        | Varchar (255) |<br/>
> | freefield4   | N        | Varchar (255) |<br/>
> | freefield5   | N        | Varchar (255) |<br/>

*Tags:* `Materials`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add values
> This api is used to sync materials with WorkorderApp.<br/>
> Each material record can contain the following data:<br/>
> <br/>
> | Parameter    | Required | Type (size)   |<br/>
> |--------------|----------|---------------|<br/>
> | code         | Y        | Varchar (255) |<br/>
> | description  | Y        | Text (64kb)   |<br/>
> | price        | Y        | Decimal       |<br/>
> | unit         | Y        | Varchar (255) |<br/>
> | eancode      | N        | Varchar (55)  |<br/>
> | barcode      | N        | Varchar (55)  |<br/>
> | freefield1   | N        | Varchar (255) |<br/>
> | freefield2   | N        | Varchar (255) |<br/>
> | freefield3   | N        | Varchar (255) |<br/>
> | freefield4   | N        | Varchar (255) |<br/>
> | freefield5   | N        | Varchar (255) |<br/>

*Tags:* `Values`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `val_entity` - _required_
* `val_primary` - _required_
* `val_column` - _required_
* `val_value_15` - _required_
* `Accept` - _required_

### Add forms
> This api is used to sync external forms with WorkorderApp.<br/>
> Each form record can contain the following data:<br/>
> <br/>
> | Parameter | Description                          | Required | Type (size)   |<br/>
> |-----------|--------------------------------------|----------|---------------|<br/>
> | name      | Name of the form                     | Y        | Varchar (255) |<br/>
> | data      | JSON data of the form                | N        | Text (64kb)   |<br/>
> | template  | HTML template to display data in PDF | N        | Text (64kb)   |<br/>
> <br/>
> <br/>
> The `data` parameters contains a JSON encoded representation of the form. The main element is called `fields` and contains an array of JSON objects representing a `field`.<br/>
> Each field contains the following data:<br/>
> <br/>
> | Parameter | Description |<br/>
> |---------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|<br/>
> | label | The label of the field. |<br/>
> | field_type | The Type of the field. Can be `text`, `checkboxes`, `radio` , `dropdown` or `signature`. |<br/>
> | required | This field indicates if the field is required to complete. Text: Field is valid a value is filled. Checkboxes: Field is valid when all the boxes are checked. Radio: Field is valid when a option is checked. Dropdown: Field is valid when a option is selected. Signature: Field is valid when a signature is set |<br/>
> | cid | Unique indentification of the field. |<br/>
> | field_options | Array containing field options. See description below. |<br/>
> <br/>
> Each field_options contains the following data:<br/>
> <br/>
> |Parameter | Description |<br/>
> |-----------------|-------------------------------------------------------------------------------------------------|<br/>
> |--------------- | ----------------------------------------------------------------------------------------------- |<br/>
> |options | The options of the field. Used in `checkboxes`, `radio` , `dropdown`. See decription below |<br/>
> |value | Value added in `text` field or base64 encoded image in `signature` field. |<br/>
> <br/>
> Each options contains the following data<br/>
> <br/>
> | Parameter | Description |<br/>
> |-----------------|-------------------------------------------------------------------------------------|<br/>
> | --------------- | ----------------------------------------------------------------------------------- |<br/>
> | checked | Indicated if options is selected. Used in `checkboxes`, `radio` , `dropdown`. |<br/>
> | label | Label for the option |<br/>
> <br/>
> + Sample JSON<br/>
>     + Text:` {<br/>
>       "label": "Serienummer",<br/>
>       "field_type": "text",<br/>
>       "required": true,<br/>
>       "field_options": {<br/>
>         "size": "small",<br/>
>         "value": ""<br/>
>       },<br/>
>       "cid": "c6"<br/>
>     }` <br/>
>     + Radio: ` {<br/>
>       "label": "Type pomp",<br/>
>       "field_type": "radio",<br/>
>       "required": true,<br/>
>       "field_options": {<br/>
>         "options": [<br/>
>           {<br/>
>             "label": "type A",<br/>
>             "checked": false<br/>
>           },<br/>
>           {<br/>
>             "label": "type B",<br/>
>             "checked": false<br/>
>           },<br/>
>           {<br/>
>             "label": "type C",<br/>
>             "checked": false<br/>
>           }<br/>
>         ]<br/>
>       },<br/>
>       "cid": "c2"<br/>
>     }`<br/>
>     + Checkboxes: ` {<br/>
>       "label": "Type pomp",<br/>
>       "field_type": "checkboxes",<br/>
>       "required": true,<br/>
>       "field_options": {<br/>
>         "options": [<br/>
>           {<br/>
>             "label": "type A",<br/>
>             "checked": false<br/>
>           },<br/>
>           {<br/>
>             "label": "type B",<br/>
>             "checked": false<br/>
>           },<br/>
>           {<br/>
>             "label": "type C",<br/>
>             "checked": false<br/>
>           }<br/>
>         ]<br/>
>       },<br/>
>       "cid": "c2"<br/>
>     }`<br/>
>     + Dropdown: ` {<br/>
>       "label": "Dropdown",<br/>
>       "field_type": "dropdown",<br/>
>       "required": true,<br/>
>       "field_options": {<br/>
>         "options": [<br/>
>           {<br/>
>             "label": "A",<br/>
>             "checked": false<br/>
>           },<br/>
>           {<br/>
>             "label": "B",<br/>
>             "checked": false<br/>
>           }<br/>
>         ],<br/>
>         "include_blank_option": false<br/>
>       },<br/>
>       "cid": "c10"<br/>
>     }`<br/>
>     + Signature: `{<br/>
>       "cid": "c5",<br/>
>       "field_options": {<br/>
>         "value": "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\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA\nAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAW9D/A4B7ViPrMDeYAAAAAElF\nTkSuQmCC\n"<br/>
>       },<br/>
>       "field_type": "signature",<br/>
>       "label": "Naamloos",<br/>
>       "required": true<br/>
>     }`<br/>

*Tags:* `Forms`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### TimeSheet - Expenses  - Add expenses

*Tags:* `TimeSheet Expenses`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `key[]` - _required_
* `value[]` - _required_
* `operator[]` - _required_
* `test` - _required_
* `Accept` - _required_

### TimeSheet - Travel - Add travel

*Tags:* `TimeSheet Travel`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `key[]` - _required_
* `value[]` - _required_
* `operator[]` - _required_
* `test` - _required_
* `Accept` - _required_

### TimeSheet - Hours - Add hours

*Tags:* `TimeSheet Hours`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `key[]` - _required_
* `value[]` - _required_
* `operator[]` - _required_
* `test` - _required_
* `Accept` - _required_

### Notes - Add note

*Tags:* `Notes`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Post locations
> This api is used to get the locations of connected devices from WorkorderApp or post locations for certain identifiers. An identifier can be anything, for example employee nr or license plate. When posting a location the type should be specified.<br/>
> Post data should contain an array with objects containing the following parameters:<br/>
> <br/>
> | Parameter                 | Description                                                       | <br/>
> |---------------------------|-------------------------------------------------------------------|  <br/>
> | lat                       | Latitude                                                          |  <br/>
> | long                      | Longitude                                                         |  <br/>
> | identifier                | Unique identifier, for example employee number or license plate.  |  <br/>
> | type                      | 0 for employee, 1 for car                                         |<br/>

*Tags:* `Locations`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Expense categories - Add
> This api is used to fetch addresses based on a filter. <br/>
> Filters can be given by adding a key and values array to the URL.<br/>
> Adding a single filter: &key=key1&value=value1<br/>
> Adding multiple filters: &key[]=key1&value[]=value1&key[]=key2&value[]=value2<br/>

*Tags:* `Expense categories`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `test` - _required_
* `Accept` - _required_

### Add worktypes
> This api is used to sync  worktypes with WorkorderApp.<br/>
> Each worktype record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                       | Required | Type (size)   |<br/>
> |---------------------------|-----------------------------------|----------|---------------|<br/>
> | wrt_name                  | Name                              | Y        | Varchar (255) |<br/>
> | wrt_description           | Description                       | Y        | Varchar (255) |<br/>
> | wrt_default_minutes       | Default minutes used for planning | Y        | Int (10) |<br/>
> | wrt_active                | Indicates if worktype is active   | Y        | Int (10)      |<br/>

*Tags:* `Worktypes`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add priorities
> This api is used to sync priorities with WorkorderApp.<br/>
> Each priority record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                                                                         | Required | Type (size)   |<br/>
> |---------------------------|-------------------------------------------------------------------------------------|----------|---------------|<br/>
> | code                      | Unique code                                                                         | Y        | Varchar (255) | <br/>
> | description               | Description of the priority. The employee can edit this when added to a work order. | Y        | Varchar (255) | <br/>
> | app_enabled               | Indication if the priority should be visible in the app                             | N        | Integer (11)  |<br/>

*Tags:* `Priorities`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add errors
> This api is used to sync errors with WorkorderApp.<br/>
> Each error record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                                                                         | Required | Type (size)   |<br/>
> |---------------------------|-------------------------------------------------------------------------------------|----------|---------------|<br/>
> | code                      | Unique code                                                                         | Y        | Varchar (255) | <br/>
> | description               | Description of the error. The employee can edit this when added to a work order. | Y        | Varchar (255) | <br/>
> | app_enabled               | Indication if the error should be visible in the app                             | N        | Integer (11)  |<br/>

*Tags:* `Errors`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add solutions
> This api is used to sync solutions with WorkorderApp.<br/>
> Each solution record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                                                                         | Required | Type (size)   |<br/>
> |---------------------------|-------------------------------------------------------------------------------------|----------|---------------|<br/>
> | code                      | Unique code                                                                         | Y        | Varchar (255) | <br/>
> | description               | Description of the solution. The employee can edit this when added to a work order. | Y        | Varchar (255) | <br/>
> | app_enabled               | Indication if the solution should be visible in the app                             | N        | Integer (11)  |<br/>

*Tags:* `Solutions`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add paymentmethods
> This api is used to sync paymentmethods with WorkorderApp.<br/>
> Each paymentmethods record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                       | Required | Type (size)   |<br/>
> |---------------------------|-----------------------------------|----------|---------------|<br/>
> | pmd_description           | Description                       | Y        | Varchar (255) |<br/>

*Tags:* `Paymentmethods`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add regions
> This api is used to sync regions with WorkorderApp.<br/>
> Each region record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description               | Required | Type (size)   |<br/>
> |---------------------------|---------------------------|----------|---------------|<br/>
> | reg_code                  | Unique code               | Y        | Varchar (255) | <br/>
> | reg_name                  | Name of the region.       | Y        | Varchar (255) | <br/>
> | reg_zip_start             | Zip start of the region.  | N        | Integer (11) | <br/>
> | reg_zip_end               | Zip end of the region.    | N        | Integer (11) | <br/>
> | reg_city                  | City of the region.       | N        | Varchar (255) | <br/>
> | reg_country               | Country of the region.    | N        | Varchar (255) |<br/>

*Tags:* `Regions`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add vehicles
> This api is used to sync vehicles with WorkorderApp.<br/>
> Each vehicle record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                                                                         | Required | Type (size)   |<br/>
> |---------------------------|-------------------------------------------------------------------------------------|----------|---------------|<br/>
> | veh_license_plate         | Unique  license plate                                                                 | Y        | Varchar (255) | <br/>
> | veh_title               | Title of the vehicle | Y        | Varchar (255) | <br/>
> | veh_brand               | Brand of the vehicle  | N        | Varchar (255) | <br/>
> | veh_model               |  Model of the vehicle| N        | Varchar (255) | <br/>
> | veh_type               | Type of the vehicle. | N        | Varchar (255) | <br/>
> | veh_image               | Url of the image . POST: An external url should be provided.  GET: You will receive a workorderapp url.    | Y        |   | <br/>
> | veh_driver               | Driver of the vehicle. This us a reference to the employee number | N        | Varchar (255) | <br/>
> | veh_driving               | Indication if the vehicle is driving. When the value is set to 1 it will be shown in the planbord. | N        | Integer (11) | <br/>
> | veh_active               | Indication if the vehicle is active                             | N        | Integer (11)  |<br/>

*Tags:* `Vehicles`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add warehouses
> This api is used to sync vehicles with WorkorderApp.<br/>
> Each vehicle record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                                                                         | Required | Type (size)   |<br/>
> |---------------------------|-------------------------------------------------------------------------------------|----------|---------------|<br/>
> | veh_license_plate         | Unique  license plate                                                                 | Y        | Varchar (255) | <br/>
> | veh_title               | Title of the vehicle | Y        | Varchar (255) | <br/>
> | veh_brand               | Brand of the vehicle  | N        | Varchar (255) | <br/>
> | veh_model               |  Model of the vehicle| N        | Varchar (255) | <br/>
> | veh_type               | Type of the vehicle. | N        | Varchar (255) | <br/>
> | veh_image               | Url of the image . POST: An external url should be provided.  GET: You will receive a workorderapp url.    | Y        |   | <br/>
> | veh_driver               | Driver of the vehicle. This us a reference to the employee number | N        | Varchar (255) | <br/>
> | veh_driving               | Indication if the vehicle is driving. When the value is set to 1 it will be shown in the planbord. | N        | Integer (11) | <br/>
> | veh_active               | Indication if the vehicle is active                             | N        | Integer (11)  |<br/>

*Tags:* `Warehouses`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add material_types
> This api is used to sync material types with WorkorderApp.<br/>
> Each material type record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                                                                         | Required | Type (size)   |<br/>
> |---------------------------|-------------------------------------------------------------------------------------|----------|---------------|<br/>
> | code                      | Unique code                                                                         | Y        | Varchar (255) | <br/>
> | description               | Description of the material type.  | Y        | Varchar (255) | <br/>
> | app_enabled               | Indication if the material type should be visible in the app                             | N        | Integer (11)  |<br/>

*Tags:* `Material types`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add workstatusses
> This api is used to sync workstatusses with WorkorderApp.<br/>
> Each workstatusses record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                       | Required | Type (size)   |<br/>
> |---------------------------|-----------------------------------|----------|---------------|<br/>
> | sta_code                  | Code                              | Y        | Varchar (255) | <br/>
> | sta_name                  | Name                              | Y        | Varchar (255) |<br/>

*Tags:* `Workstatusses`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add addresses
> This api is used to sync addresses with WorkorderApp. An address should always be related to a certain client and can have a main contact person associated with it.<br/>
> `adr_code` is used as a unique reference to either insert or update the address.<br/>
> Each address record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                                                                 | Required | Type (size)   |<br/>
> |---------------------------|-----------------------------------------------------------------------------|----------|---------------|<br/>
> | adr_debtor_nr             | Debtor number of the relation                                               | Y        | Varchar (255) |<br/>
> | adr_code                  | Unique code of the address. Used as reference in the workorder.             | Y        | Varchar (255) |<br/>
> | adr_cpn_code              | Contact person code of the address                                          | N        | Varchar (255) |<br/>
> | adr_line_1                | Address line. Usually street and number.                                    | Y        | Varchar (255) |<br/>
> | adr_zip                   | Zipcode of the address                                                      | Y        | Varchar (255) |<br/>
> | adr_city                  | City of the adress                                                          | Y        | Varchar (255) |<br/>
> | adr_country               | Country of the address                                                      | N        | Varchar (255) |<br/>
> | adr_remark                | Remark of the address                                                       | N        | Varchar (255) |<br/>

*Tags:* `Addresses`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add parts
> This api is now deprecated. Use materials to register the parts of certain objects.<br/>
> This api is used to sync parts with WorkorderApp.<br/>
> Each part record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                                                                                                               | Required | Type (size)   |<br/>
> |---------------------------|---------------------------------------------------------------------------------------------------------------------------|----------|---------------|<br/>
> | prt_code                  | Unique code of the parts. Used as reference for other entities                                                         | Y        | Varchar (255) |<br/>
> | prt_name                  | Part name/description name                                                                                                             | Y        | Varchar (255) |<br/>
> | prt_sup_code              | Supplier code                                                                                                             | Y        | Varchar (255) |<br/>
> | prt_value                 | Value of a parts                                                                                                             | Y        | Varchar (255) |<br/>
> | prt_image                 | Url of the image name. POST: An external url should be provided.  GET: You will receive a workorderapp url.     | N        | Varchar (255)      |<br/>

*Tags:* `Parts`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add object parts
> This api is used to sync object parts with WorkorderApp.<br/>
> The result can be filtered by using the advanced filter. As described in the introduction section. Allowed columns: `opr_obj_code` `opr_prt_code` `opr_serial_number`<br/>
> Each object_part record can contain the following data:<br/>
> <br/>
> | Parameter                         | Description                                           | Required | Type (size)   |<br/>
> |-----------------------------------|-------------------------------------------------------|----------|---------------|<br/>
> | opr_obj_code                      | Object code                                           | Y        | Varchar (255) |<br/>
> | opr_prt_code                      | Object part (Artikelcode from items in materials)     | Y        | Varchar (255) |<br/>
> | opr_serial_number                 | Serial number of parts used in object                 | N        | Varchar (255) |<br/>
> | opr_amount                        | Amount of parts used in object                        | Y        | Int (10)      |<br/>
> | opr_timestamp_installation        | Date of installing (Y-m-d)                            | N        | Date       |<br/>
> | opr_warranty_months               | Amount of months, used to calculate expiration date.  | N        | Int (10)      |<br/>
> | opr_timestamp_warranty_expires    | Warranty expiration date, automatically calculated based on installation date and the warranty months    | N        | Varchar (255)      |<br/>
> | val_value_1                       | Freefield value 1                                     | N        | Varchar (255)      |<br/>
> | val_value_2  - val_value_20       | Freefield value 2  till 20                            | N        | Varchar (255)      |<br/>

*Tags:* `Object parts`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Post workorders
> This api is used to post one or more workorders to WorkorderApp.<br/>
> A workorder can contain the following data:<br/>
> <br/>
> | Parameter                    | Detail                                                                                                     | Required | Type (size)   |<br/>
> |------------------------------|------------------------------------------------------------------------------------------------------------|----------|---------------|<br/>
> | WorkorderNo                  | Unique number from ERP/CRM                                                                                 | Yes      | Varchar (255) |<br/>
> | ProjectNr                    | Internal Project number                                                                                    | No       | Varchar (255) |<br/>
> | ExternProjectNr              | External Project number                                                                                    | No       | Varchar (255) |<br/>
> | CustomerName                 | Customer name                                                                                              | Yes      | Varchar (255) |<br/>
> | CustomerDebtorNr             | Customer Debtor number                                                                                     | Yes      | Varchar (255) |<br/>
> | CustomerStreet               | Customer street                                                                                            | Yes      | Varchar (255) |<br/>
> | CustomerStreetNo             | Customer street number                                                                                     | No       | Varchar (255) |<br/>
> | CustomerEmail                | Customer Email                                                                                             | No       | Varchar (255) |<br/>
> | CustomerZIP                  | Customer zip code                                                                                          | Yes      | Varchar (255) |<br/>
> | CustomerCity                 | Customer city                                                                                              | Yes      | Varchar (255) |<br/>
> | CustomerContactPerson        | Customer contact person                                                                                    | Yes      | Varchar (255) |<br/>
> | CustomerPhone                | Customer phone number                                                                                      | No       | Varchar (255) |<br/>
> | CustomerRemark               | Customer remark                                                                                            | No       | Text (64kb)   |<br/>
> | CustomerLatitude             | Latitude of work location, used for navigation and to display on maps.                                     | No       | Float(10,6)   |<br/>
> | CustomerLongitude            | Longitude of work location, used for navigation and to display on maps.                                    | No       | Float(10,6)   |<br/>
> | CustomerNameInvoice          | Invoice customer name                                                                                      | Yes      | Varchar (255) |<br/>
> | CustomerDebtorNrInvoice      | Invoice customer debtor number                                                                             | Yes      | Varchar (255) |<br/>
> | CustomerStreetInvoice        | Invoice customer street name                                                                               | Yes      | Varchar (255) |<br/>
> | CustomerStreetNoInvoice      | Invoice customer street number                                                                             | No       | Varchar (255) |<br/>
> | CustomerEmailInvoice         | Invoice customer email                                                                                     | No       | Varchar (255) |<br/>
> | CustomerZIPInvoice           | Invoice customer zip code                                                                                  | Yes      | Varchar (255) |<br/>
> | CustomerCityInvoice          | Invoice customer city                                                                                      | Yes      | Varchar (255) |<br/>
> | CustomerContactPersonInvoice | Invoice customer contact person                                                                            | Yes      | Varchar (255) |<br/>
> | CustomerPhoneInvoice         | Invoice customer phone number                                                                              | No       | Varchar (255) |<br/>
> | CustomerRemarkInvoice        | Invoice customer remark                                                                                    | No       | Text (64kb)   |<br/>
> | TypeOfWork                   | Installatie, Garantie, Levering, Onderhoud, Project, Regie, Reparatie,  Service, Storing, Verkoop, Verhuur | Yes      | Varchar (255) |<br/>
> | WorkDescription              | Work description of the workorder. Visible for customer when signing and when receiving the PDF.           | No       | Text (64kb)   |<br/>
> | InternalWorkDescription      | Internal work description of the workorder. Only visible for the employee                                  | No       | Text (64kb)   |<br/>
> | PaymentMethod                | niet van toepassing, op rekening, contact voldaan, pin betaling, conform offerte                           | Yes      | Varchar (255) |<br/>
> | EmployeeNr                   | Employee Number                                                                                            | No       | Varchar (255) |<br/>
> | WorkDate                     | Scheduled date for work (d-m-Y)                                                                            | No       | Varchar (255) |<br/>
> | WorkTime                     | Scheduled time for work (H:i)                                                                              | No       | Varchar (255) |<br/>
> | WorkEndDate                  | Scheduled end date for work (d-m-Y)                                                                        | No       | Varchar (255) |<br/>
> | WorkEndTime                  | Scheduled end time for work (H:i)                                                                          | No       | Varchar (255) |<br/>
> | WorkDeadline                 | Scheduled deadline for the workorder.                                                                      | No       | Varchar (255) |<br/>
> | WorkDuration                 | Duration of the workorder (in minutes). Used to fill WorkEndDate and WorkEndTime based on WorkDate and WorkTime.        | No       | Integer   |<br/>
> | WorkStatus                   | Internal work status code. Can be added through status API.                                                | No       | Varchar (255) |<br/>
> | PickupPlanning               | Indication if the work order should be added to batch to be picked up. Value should be 0 or 1.             | No       | Integer       |<br/>
> | WebPlanning                  | Indication if webplanning is enabled for this order.                                                       | No       | Integer       |<br/>
> | CpnCode                      | Contact person code                                                                                        | No       | Varchar (255) |<br/>
> | AdrCode                      | Address code                                                                                               | No       | Varchar (255) |<br/>
> | ShortWorkDescription         | Short work description. For example 1 line to show in an overview                                          | No       | Varchar (255) |<br/>
> | Comment                      | Additional field for the employee to leave their comment                                                   | No       | Varchar (255) |<br/>
> | ErrorCode                    | Selected code as added in the errors API                                                                   | No       | Varchar (255) |<br/>
> | ErrorMessage                 | Message corresponding to the selected Error, can be changed by the employee                                | No       | Varchar (255) |<br/>
> | SolutionCode                 | Selected code as added in the solutions API                                                                | No       | Varchar (255) |<br/>
> | SolutionMessage              | Message corresponding to the selected Solution, can be changed by the employee                             | No       | Varchar (255) |<br/>
> | PriorityCode                 | Selected code as added in the priorities API                                                               | No       | Varchar (255) |<br/>
> | PriorityMessage              | Message corresponding to the selected Priority, can be changed by the employee                             | No       | Varchar (255) |<br/>
> | MinimumHours                 | Minimum amount of hours that the customer should sign for. For example: The customer should always sign for 2 hours. If the employee only registers 25 minutes the customer still gets to see 2 hours.                | No       | Decimal (7,2) |<br/>
> | RoundingAmount               | Amount of minutes that the total time should be rounded to. For exammple: Your company only works with amounts of 30 minutes. If the user only registers 40 minutes the customer will have to sign for 60 minutes.                | No       | Varchar (255) |<br/>
> | Attachments                  | An array containing multiple files. See specification below.                                               | No       | Array         |<br/>
> | Materials                    | An array containing material rows. See specification below.                                                | No       | Array         |<br/>
> | Workperiods                  | An array containing workperiod rows. See specification below.                                              | No       | Array         |<br/>
> | Forms                        | Array of forms. Each row contains Name, Data and ObjectCode                                                | No       | Array         |<br/>
> | Employees                    | Array of employee numbers.                                                                                 | No       | Array         |<br/>
> | WorkObjects                  | Array of objects codes.                                                                                    | No       | Array         |<br/>
> <br/>
> Attachments specification<br/>
> <br/>
> | Parameter | Detail                                                                                        | Required | Type (size)   |<br/>
> |-----------|-----------------------------------------------------------------------------------------------|----------|---------------|<br/>
> | File      | URL of the attachment file. This has to be an existing file. The file is saved on our server. | No       | Varchar (255) |<br/>
> | Data      | Base64 encoded file data.                                                                     | No       | Base64        |<br/>
> | FileName  | Filename of the Base64 encoded data.                                                          | No       | Varchar (255) |<br/>
> <br/>
> An attachment can be added by providing a valid URL or by providing Base64 encoded data and filename.<br/>
> Material specification<br/>
> <br/>
> | Parameter     | Detail                                                             | Required | Type          |<br/>
> |---------------|--------------------------------------------------------------------|----------|---------------|<br/>
> | MaterialCode  | Article number, code or barcode of this material. Example: A786878 | Yes      | Varchar (255) |<br/>
> | MaterialNr    | Amount of this material used. Example: 1                           | Yes      | Decimal       |<br/>
> | MaterialPrice | Price of this material. Example: 0,00                              | Yes      | Decimal       |<br/>
> | MaterialName  | Material name and/or description. Example: Kleinmateriaal          | Yes      | Varchar (255) |<br/>
> | MaterialUnit  | Unit of this material. Example: M2                                 | No       | Varchar (255) |<br/>
> | MaterialType  | User defined material type                                         | No       | Varchar (255) |<br/>
> | MaterialFreeField1  | User defined field 1                                         | No       | Varchar (255) |<br/>
> | MaterialFreeField2  | User defined field 2                                         | No       | Varchar (255) |<br/>
> | MaterialFreeField3  | User defined field 3                                         | No       | Varchar (255) |<br/>
> | MaterialFreeField4  | User defined field 4                                         | No       | Varchar (255) |<br/>
> | MaterialFreeField5  | User defined field 5                                         | No       | Varchar (255) |<br/>
> <br/>
> Workperiod specification<br/>
> <br/>
> | Parameter     | Detail                                                    | Required  | Type          |<br/>
> |---------------|-----------------------------------------------------------|-----------|---------------|<br/>
> | WorkDate      | Date specified in d-m-Y                                   | Yes       | Varchar (255) |<br/>
> | BeginTime     | Time specified in H:i                                     | Yes       | Varchar (255) |<br/>
> | EndTime       | Time specified in H:i                                     | Yes       | Varchar (255) |<br/>
> | Break         | Break time in minutes                                     | No        | Int (11)      |<br/>
> | TotalTime     | Sum of EndTime - BeginTime - Break formatted in H:i       | Yes       | Varchar (255) |<br/>
> | Travel        | Travel distance                                           | No        | Int (11)      |<br/>
> | WorkRemark    | Work remark                                               | No        | Text          |<br/>
> | HourType      | Hour type code                                            | No        | Varchar (55)  |<br/>
> | EmployeeNr    | Employee nunber                                           | No        | Varchar (55)  |<br/>
> <br/>
> Example array:<br/>
> ``` json<br/>
> "Workperiods": [<br/>
>     {<br/>
>         "BeginTime": "08:30",<br/>
>         "TotalTime": "03:45",<br/>
>         "WorkRemark": "",<br/>
>         "WorkDate": "26-09-2013",<br/>
>         "EndTime": "12:15",<br/>
>         "Travel": "1",<br/>
>         "EmployeeNr":"11",<br/>
>         "HourType":"001"<br/>
>     }<br/>
> ] <br/>
> ```<br/>
> Forms specification<br/>
> <br/>
> | Parameter     | Detail                                                                                                                                | Required | Type          |<br/>
> |---------------|---------------------------------------------------------------------------------------------------------------------------------------|----------|---------------|<br/>
> | Name          | Name of the form. Will be visible to employee and used to search for data.                                                            | Yes      | Varchar (255) |<br/>
> | Data          | JSON data of the Form elements. See forms API for description. When this is empty we will use the name to lookup a predefined form.   | No      | Text (64kb)    |<br/>
> | ObjectCode    | Object connected to the form. We will search our list of object for the corresponding object.                                         | No      | Varchar (255)  |<br/>

*Tags:* `Work Orders`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### UpdateWorkorder (Materials)
> This API is used to update an existing workorder. The row_id of workorder_no can be used to identify the specific workorder.<br/>

*Tags:* `Work Orders`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `row_id` - _required_
* `ClearMaterials` - _required_
* `ProcessMaterials` - _required_
* `Accept` - _required_

### Add object
> This api is used to sync objects with WorkorderApp.<br/>
> Each object record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                                                                                                               | Required | Type (size)   |<br/>
> |---------------------------|---------------------------------------------------------------------------------------------------------------------------|----------|---------------|<br/>
> | obj_code                  | Unique code of the object. Used as reference for other entities                                                           | Y        | Varchar (255) |<br/>
> | obj_sup_code              | Supplier code. Used as reference to supplier entity                                                                       | N        | Varchar (255) |<br/>
> | obj_debiteur_nummer       | Debtor number. Used as reference to customer clients.                                                                     | Y        | Varchar (255) |<br/>
> | obj_adr_code              | Address code. Used as a reference to the addres of a customer client.                                                     | N        | Varchar (255) |<br/>
> | obj_obj_code              | Parent object code.                                                                                                       | N        | Varchar (255) |<br/>
> | obj_image                 | Url of the image name. POST: An external url should be provided.  GET: You will receive a workorderapp url.               | N        | Varchar (255) |<br/>
> | obj_description           | Description of the object                                                                                                 | Y        | Varchar (255) |<br/>
> | obj_price                 | Price of the object                                                                                                       | N        | Decimal (7,2) |<br/>
> | obj_floor_level           | Floor level of the object                                                                                                 | N        | Int (10)      |<br/>
> | obj_location              | Textual description of the location of the object                                                                         | N        | Varchar (255) |<br/>
> | obj_latitude              | Latitude of the location of the object                                                                                    | N        | Float (10,6)  |<br/>
> | obj_longitude             | Longitude of the location of the object                                                                                   | N        | Float (10,6)  |<br/>
> | obj_type                  | Type                                                                                                                      | N        | Varchar (255) |<br/>
> | obj_model                 | Model                                                                                                                     | N        | Varchar (255) |<br/>
> | obj_brand                 | Brand                                                                                                                     | N        | Varchar (255) |<br/>
> | obj_date_warranty_expires | Expiration date of the warranty                                                                                           | N        | Varchar (255) |<br/>
> | obj_serialnumber          | Serialnumber of the object                                                                                                | N        | Varchar (255) |<br/>
> | obj_date_last_inspection  | Date of last inspection                                                                                                   | N        | Varchar (255) |<br/>
> | obj_date_installation     | Date of installation                                                                                                      | N        | Varchar (255) |<br/>
> | obj_freefield_1           |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_2           |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_3           |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_4           |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_5           |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_6           |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_7           |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_8           |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_9           |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_10          |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_11          |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_12          |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_13          |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_14          |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_15          |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_16          |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_17          |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_18          |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_19          |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_freefield_20          |                                                                                                                           | N        | Varchar (255) |<br/>
> | obj_order                 | Sort order of an object                                                                                                   | N        | Int (10)      |<br/>
> | obj_created               | Timestamp of creating                                                                                                     | N        | DateTime      |<br/>
> | obj_modified              | Timestamp of modifying                                                                                                    | N        | DateTime      |<br/>

*Tags:* `Objects`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add suppliers
> This api is used to sync suppliers with WorkorderApp.<br/>
> Each supplier record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                                                                                                               | Required | Type (size)   |<br/>
> |---------------------------|---------------------------------------------------------------------------------------------------------------------------|----------|---------------|<br/>
> | sup_code                  | Unique code of the supplier. Used as reference for other entities                                                         | Y        | Varchar (255) |<br/>
> | sup_name                  | Supplier name                                                                                                             | Y        | Varchar (255) |<br/>
> | sup_image                 | Url of the image name. POST: An external url should be provided.  GET: You will receive a workorderapp url.               | N        | Varchar (255)      |<br/>

*Tags:* `Suppliers`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add freefields
> This api is used to sync suppliers with WorkorderApp.<br/>
> Each supplier record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                                                                                                               | Required | Type (size)   |<br/>
> |---------------------------|---------------------------------------------------------------------------------------------------------------------------|----------|---------------|<br/>
> | sup_code                  | Unique code of the supplier. Used as reference for other entities                                                         | Y        | Varchar (255) |<br/>
> | sup_name                  | Supplier name                                                                                                             | Y        | Varchar (255) |<br/>
> | sup_image                 | Url of the image name. POST: An external url should be provided.  GET: You will receive a workorderapp url.               | N        | Varchar (255)      |<br/>

*Tags:* `Freefields`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Update quotation
> This api is used to fetch generated invoices from WorkorderApp.<br/>
> The result can be filtered by using the advanced filter. As described in the introduction section.<br/>
> <br/>
> | Parameter                 | Description                                                                                           |<br/>
> |---------------------------|-------------------------------------------------------------------------------------------------------|<br/>
> | inv_id                    | Unique invoice ID  number of the invoice                                                              |<br/>
> | inv_worksheet_id          | Worksheet ID that is used to generate this invoice                                                    |<br/>
> | inv_quo_id                | Quotation ID that is used to generate this invoice                                                    |<br/>
> | inv_inv_id                | Parent invoice ID. Used when creating a credit invoice.                                               |<br/>
> | inv_type                  | Invoice type, can be DEBIT, CREDIT, CONCEPT_DEBIT or CONCEPT_CREDIT                                   |<br/>
> | inv_currency_code         | ISO 4217 currency code                                                                                |<br/>
> | inv_currency_symbol       | Currency symbol shown in the UI                                                                       |<br/>
> | inv_description           | Description of the invoice                                                                            |<br/>
> | inv_invoice_debtor_nr     | Debtor number of the assigned relation                                                                |<br/>
> | inv_invoice_debtor_name   | Debtor name of the assigned relation                                                                  |<br/>
> | inv_invoice_debtor_email  | Debtor e-mail of the assigned relation                                                                |<br/>
> | inv_number_numeric        | Invoice number numeric value                                                                          |<br/>
> | inv_number_formatted      | Pretty formatted invoice number                                                                       |<br/>
> | inv_status                | Invoice status, can be OPEN, PAYED, OVERDUE, REMINDER_1, REMINDER_2, REMINDER_3 or ...                |<br/>
> | inv_reference             | Reference, example purchase order number workorder number                                             |<br/>
> | inv_date                  | Invoice date                                                                                          |<br/>
> | inv_due_date              | Invoice due date                                                                                      |<br/>
> | inv_due_days              | Amount of due days. This days are added to the inv_date to calculate the inv_due_date.                |<br/>
> | inv_terms                 | Terms shown in the footer of the PDF.                                                                 |<br/>
> | inv_header                | Header shown on top of the PDF.                                                                       |<br/>
> | inv_amount                | Total amount including VAT.                                                                           |<br/>
> | inv_amount_excl           | Total amount excluding VAT.                                                                           |<br/>
> | inv_balance               | Total amounts of the transactions registered to this invoice.                                         |<br/>
> | inv_user_create           | User who created this invoice                                                                         |<br/>
> | inv_user_mutate           | User who mutated this invoice                                                                         |<br/>
> | inv_user_send             | User who marked this invoice as send.                                                                 |<br/>
> | inv_timestamp_create      | Timestamp of creation                                                                                 |<br/>
> | inv_timestamp_mutate      | Timestamp of mutating                                                                                 |<br/>
> | inv_timestamp_payed       | Timestamp when the invoice was marked as payed (inv_amount equal to inv_balance)                      |<br/>
> | inv_timestamp_send        | Timestamp of marking the invoice as send.                                                             |<br/>
> | iln_lines                 | Array of invoice lines.                                                                               |<br/>
> | invoice_debtor            | Invoice debtor.                                                                                       |<br/>
> | pdf                       | Temporary PDF url.                                                                                    |<br/>
> | ubl                       | Temporary ubl 2.0 url.                                                                                |<br/>
> <br/>
> Invoice line parameters<br/>
> <br/>
> | Parameter             | Description                                      |<br/>
> |-----------------------|--------------------------------------------------|<br/>
> | iln_id                | Line ID                                          |<br/>
> | iln_inv_id            | Invoice Id                                       |<br/>
> | iln_order             | Position of the line                             |<br/>
> | iln_material_code     | Material code                                    |<br/>
> | iln_material_hourtype | Hourtype code                                    |<br/>
> | iln_description       | Line description                                 |<br/>
> | iln_amount            | Line amount                                      |<br/>
> | iln_price             | Item price                                       |<br/>
> | iln_vat_percentage    | Vat percentage                                   |<br/>
> | iln_discount          | Discount percentage                              |<br/>
> | iln_total             | Total price excluding vat and discount           |<br/>
> | iln_total_discount    | Calculated discount amount                       |<br/>
> | iln_total_vat         | Calculated vat amount                            |<br/>
> | iln_total_excl        | Total price excluding vat and including discount |<br/>
> | iln_total_incl        | Total price including vat and including discount |<br/>

*Tags:* `Quotations`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `key` - _required_
* `value` - _required_
* `operator` - _required_
* `Accept` - _required_

### Post Prices
> This api is used to fetch generated quotations from WorkorderApp.<br/>
> The result can be filtered by using the advanced filter. As described in the introduction section.<br/>

*Tags:* `Prices`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `test` - _required_
* `Accept` - _required_

### Update invoice
> This api is used to fetch generated invoices from WorkorderApp.<br/>
> The result can be filtered by using the advanced filter. As described in the introduction section.<br/>
> <br/>
> | Parameter                 | Description                                                                                           |<br/>
> |---------------------------|-------------------------------------------------------------------------------------------------------|<br/>
> | inv_id                    | Unique invoice ID  number of the invoice                                                              |<br/>
> | inv_worksheet_id          | Worksheet ID that is used to generate this invoice                                                    |<br/>
> | inv_quo_id                | Quotation ID that is used to generate this invoice                                                    |<br/>
> | inv_inv_id                | Parent invoice ID. Used when creating a credit invoice.                                               |<br/>
> | inv_type                  | Invoice type, can be DEBIT, CREDIT, CONCEPT_DEBIT or CONCEPT_CREDIT                                   |<br/>
> | inv_currency_code         | ISO 4217 currency code                                                                                |<br/>
> | inv_currency_symbol       | Currency symbol shown in the UI                                                                       |<br/>
> | inv_description           | Description of the invoice                                                                            |<br/>
> | inv_invoice_debtor_nr     | Debtor number of the assigned relation                                                                |<br/>
> | inv_invoice_debtor_name   | Debtor name of the assigned relation                                                                  |<br/>
> | inv_invoice_debtor_email  | Debtor e-mail of the assigned relation                                                                |<br/>
> | inv_number_numeric        | Invoice number numeric value                                                                          |<br/>
> | inv_number_formatted      | Pretty formatted invoice number                                                                       |<br/>
> | inv_status                | Invoice status, can be OPEN, PAYED, OVERDUE, REMINDER_1, REMINDER_2, REMINDER_3 or ...                |<br/>
> | inv_reference             | Reference, example purchase order number workorder number                                             |<br/>
> | inv_date                  | Invoice date                                                                                          |<br/>
> | inv_due_date              | Invoice due date                                                                                      |<br/>
> | inv_due_days              | Amount of due days. This days are added to the inv_date to calculate the inv_due_date.                |<br/>
> | inv_terms                 | Terms shown in the footer of the PDF.                                                                 |<br/>
> | inv_header                | Header shown on top of the PDF.                                                                       |<br/>
> | inv_amount                | Total amount including VAT.                                                                           |<br/>
> | inv_amount_excl           | Total amount excluding VAT.                                                                           |<br/>
> | inv_balance               | Total amounts of the transactions registered to this invoice.                                         |<br/>
> | inv_user_create           | User who created this invoice                                                                         |<br/>
> | inv_user_mutate           | User who mutated this invoice                                                                         |<br/>
> | inv_user_send             | User who marked this invoice as send.                                                                 |<br/>
> | inv_timestamp_create      | Timestamp of creation                                                                                 |<br/>
> | inv_timestamp_mutate      | Timestamp of mutating                                                                                 |<br/>
> | inv_timestamp_payed       | Timestamp when the invoice was marked as payed (inv_amount equal to inv_balance)                      |<br/>
> | inv_timestamp_send        | Timestamp of marking the invoice as send.                                                             |<br/>
> | iln_lines                 | Array of invoice lines.                                                                               |<br/>
> | invoice_debtor            | Invoice debtor.                                                                                       |<br/>
> | pdf                       | Temporary PDF url.                                                                                    |<br/>
> | ubl                       | Temporary ubl 2.0 url.                                                                                |<br/>
> <br/>
> Invoice line parameters<br/>
> <br/>
> | Parameter             | Description                                      |<br/>
> |-----------------------|--------------------------------------------------|<br/>
> | iln_id                | Line ID                                          |<br/>
> | iln_inv_id            | Invoice Id                                       |<br/>
> | iln_order             | Position of the line                             |<br/>
> | iln_material_code     | Material code                                    |<br/>
> | iln_material_hourtype | Hourtype code                                    |<br/>
> | iln_description       | Line description                                 |<br/>
> | iln_amount            | Line amount                                      |<br/>
> | iln_price             | Item price                                       |<br/>
> | iln_vat_percentage    | Vat percentage                                   |<br/>
> | iln_discount          | Discount percentage                              |<br/>
> | iln_total             | Total price excluding vat and discount           |<br/>
> | iln_total_discount    | Calculated discount amount                       |<br/>
> | iln_total_vat         | Calculated vat amount                            |<br/>
> | iln_total_excl        | Total price excluding vat and including discount |<br/>
> | iln_total_incl        | Total price including vat and including discount |<br/>

*Tags:* `Invoices`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `key` - _required_
* `value` - _required_
* `operator` - _required_
* `Accept` - _required_

### Add transactions
> This api is used to fetch a single generated invoice from WorkorderApp.<br/>
> Filters can be given by adding a key and values array to the URL.<br/>
> Adding a single filter: &key=key1&value=value1&operator=gt<br/>
> Adding multiple filters: &key[]=key1&value[]=value1&operator[]=eq&key[]=key2&value[]=value2&operator[]=gt<br/>
> <br/>
> Following operators are allowed:<br/>
> <br/>
> | Operator | Description                 |<br/>
> |----------|-----------------------------|<br/>
> | li       | Like (%)                    |<br/>
> | eq       | Equal (=)                   |<br/>
> | ne       | Not equal (!=)              |<br/>
> | gt       | Greather than (>)           |<br/>
> | ge       | Greather than or equal (>=) |<br/>
> | lt       | Less than  (<)              |<br/>
> | le       | Less than or equal (<=)     |<br/>
> Transaction parameters. The invoice id of a transaction transaction can be empty if a transaction is not assigned to an invoice. Once it is assigned the balance of the invoice will be adjusted.<br/>
> <br/>
> | Paramter                    | Description                                | Type         |<br/>
> |-----------------------------|--------------------------------------------|--------------|<br/>
> | int_inv_id                  | Invoice ID                                 | int(11)      |<br/>
> | int_transaction_id          | Transaction ID                             | varchar(255) |<br/>
> | int_external_transaction_id | External Transaction ID                    | varchar(255) |<br/>
> | int_description             | Transaction Description                    | varchar(255) |<br/>
> | int_amount                  | Transaction amount                         | decimal(7,2) |<br/>
> | int_type                    | Transaction type                           | varchar(255) |<br/>
> | int_type_description        | Transaction type description               | varchar(255) |<br/>
> | int_status                  | Transaction status,NEW or PROCESSED        | varchar(55)  |<br/>
> | int_user                    | User/entity who registered the transaction | varchar(255) |<br/>
> | int_timestamp               | Timestamp registered                       | timestamp    |<br/>

*Tags:* `Transactions`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Update transactions
> This api is used to fetch a single generated invoice from WorkorderApp.<br/>
> Filters can be given by adding a key and values array to the URL.<br/>
> Adding a single filter: &key=key1&value=value1&operator=gt<br/>
> Adding multiple filters: &key[]=key1&value[]=value1&operator[]=eq&key[]=key2&value[]=value2&operator[]=gt<br/>
> <br/>
> Following operators are allowed:<br/>
> <br/>
> | Operator | Description                 |<br/>
> |----------|-----------------------------|<br/>
> | li       | Like (%)                    |<br/>
> | eq       | Equal (=)                   |<br/>
> | ne       | Not equal (!=)              |<br/>
> | gt       | Greather than (>)           |<br/>
> | ge       | Greather than or equal (>=) |<br/>
> | lt       | Less than  (<)              |<br/>
> | le       | Less than or equal (<=)     |<br/>
> Transaction parameters. The invoice id of a transaction transaction can be empty if a transaction is not assigned to an invoice. Once it is assigned the balance of the invoice will be adjusted.<br/>
> <br/>
> | Parameter                    | Description                                | Type         |<br/>
> |-----------------------------|--------------------------------------------|--------------|<br/>
> | int_inv_id                  | Invoice ID                                 | int(11)      |<br/>
> | int_transaction_id          | Transaction ID                             | varchar(255) |<br/>
> | int_external_transaction_id | External Transaction ID                    | varchar(255) |<br/>
> | int_description             | Transaction Description                    | varchar(255) |<br/>
> | int_amount                  | Transaction amount                         | decimal(7,2) |<br/>
> | int_type                    | Transaction type                           | varchar(255) |<br/>
> | int_type_description        | Transaction type description               | varchar(255) |<br/>
> | int_status                  | Transaction status,NEW or PROCESSED        | varchar(55)  |<br/>
> | int_user                    | User/entity who registered the transaction | varchar(255) |<br/>
> | int_timestamp               | Timestamp registered                       | timestamp    |<br/>

*Tags:* `Transactions`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add contact persons
> This api is used to sync contact persons with WorkorderApp. A contact person should always be related to a certain client.<br/>
> `cpn_code` is used as a unique reference to either insert or update the address.<br/>
> Each address record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                                                                 | Required | Type (size)   |<br/>
> |---------------------------|-----------------------------------------------------------------------------|----------|---------------|<br/>
> | cpn_debtor_nr             | Debtor number of the relation                                               | Y        | Varchar (255) |<br/>
> | cpn_code                  | Unique code of the contact person. Used as reference in the workorder.      | Y        | Varchar (255) |<br/>
> | cpn_name                  | Name of the contact person.                                                 | Y        | Varchar (255) |<br/>
> | cpn_phone                 | Phone of the contact person.                                                | N        | Varchar (255) |<br/>
> | cpn_email                 | Email of the contact person.                                                | N        | Varchar (255) |<br/>

*Tags:* `Contactpersons`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

### Add generic_notes
> This api is used to sync contact persons with WorkorderApp. A contact person should always be related to a certain client.<br/>
> `cpn_code` is used as a unique reference to either insert or update the address.<br/>
> Each address record can contain the following data:<br/>
> <br/>
> | Parameter                 | Description                                                                 | Required | Type (size)   |<br/>
> |---------------------------|-----------------------------------------------------------------------------|----------|---------------|<br/>
> | cpn_debtor_nr             | Debtor number of the relation                                               | Y        | Varchar (255) |<br/>
> | cpn_code                  | Unique code of the contact person. Used as reference in the workorder.      | Y        | Varchar (255) |<br/>
> | cpn_name                  | Name of the contact person.                                                 | Y        | Varchar (255) |<br/>
> | cpn_phone                 | Phone of the contact person.                                                | N        | Varchar (255) |<br/>
> | cpn_email                 | Email of the contact person.                                                | N        | Varchar (255) |<br/>

*Tags:* `Generic Notes`

#### Input Parameters
* `token` - _required_
* `software_token` - _required_
* `Accept` - _required_

## License

: OutSmart<br/>
                    <br/>

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
