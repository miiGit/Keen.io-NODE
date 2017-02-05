# Getting started

## How to Build

The generated SDK relies on [Node Package Manager](https://www.npmjs.com/) (NPM) being available to resolve dependencies. If you don't already have NPM installed, please go ahead and follow instructions to install NPM from [here](https://nodejs.org/en/download/).
The SDK also requires Node to be installed. If Node isn't already installed, please install it from [here](https://nodejs.org/en/download/)
> NPM is installed by default when Node is installed

To check if node and npm have been successfully installed, write the following commands in command prompt:
* `node --version`
* `npm -version` 
![Version Check](https://apidocs.io/illustration/nodejs?step=versionCheck&workspaceFolder=Keen.io-Node)  

Now use npm to resolve all dependencies by running the following command in the root directory (of the SDK folder):
* `npm install`
![Resolve Dependencies](https://apidocs.io/illustration/nodejs?step=resolveDependency1&workspaceFolder=Keen.io-Node)
![Resolve Dependencies](https://apidocs.io/illustration/nodejs?step=resolveDependency2)

This will install all dependencies in the `node_modules` folder. 

Once dependencies are resolved, you will need to move the folder `KeenIo ` in to your `node_modules` folder.

## How to Use

The following section explains how to use the library in a new project.

### 1. Open Project Folder
Open an IDE/Text Editor for JavaScript like Sublime Text. The basic workflow presented here is also applicable if you prefer using a different editor or IDE.  
Click on `File` and select `Open Folder`
![Open Folder](https://apidocs.io/illustration/nodejs?step=openFolder)

Select the folder of your SDK and click on `Select Folder` to open it up in Sublime Text. The folder will become visible in the bar on the left.
![Open Project](https://apidocs.io/illustration/nodejs?step=openProject&workspaceFolder=Keen.io-Node)


### 2. Creating a Test File
Now right click on the folder name and select the `New File` option to create a new test file.    Save it as `index.js` Now import the generated NodeJS library using the following lines of code:
```JavaScript
var lib = require('lib');
```
Save changes.

![Create new file](https://apidocs.io/illustration/nodejs?step=createNewFile&workspaceFolder=Keen.io-Node)
![Save new file](https://apidocs.io/illustration/nodejs?step=saveNewFile&workspaceFolder=Keen.io-Node)

### 3. Running The Test File
To run the `index.js` file, open up the command prompt and navigate to the Path where the SDK folder resides. Type the following command to run the file:  
`node index.js`
![Run file](https://apidocs.io/illustration/nodejs?step=runProject&workspaceFolder=Keen.io-Node)


## How to Test

These tests use Mocha framework for testing, coupled with Chai for assertions. These dependencies need to be installed for tests to run.
Tests can be run in a number of ways:

### Method 1 
###### (Run all tests)

1. Navigate to the root directory of the SDK folder from command prompt.
2. Type `mocha --recursive` to run all the tests.

### Method 2
###### (Run all tests)

1. Navigate to the `../test/Controllers/` directory from command prompt.
2. Type `mocha *` to run all the tests.

### Method 3
###### (Run specific controller's tests)

1. Navigate to the `../test/Controllers/` directory from command prompt.
2. Type `mocha  Keen.ioController`  to run all the tests in that controller file.

> To increase mocha's default timeout, you can change the `TESTTIMEOUT` parameter's value in `Configuration.js`.  
> ***NOTE:*** Changing default timeout is available for only Binary/File type endpoint tests

![Run Tests](https://apidocs.io/illustration/nodejs?step=runTests&controllerName=Keen.ioController)

## Initialization

### Authentication
In order to setup authentication and initialization of the API client, you need the following information.

| Parameter | Description |
|-----------|-------------|
| authorization | its value should just be your API Key |



API client can be initialized as following:

```JavaScript
// Configuration parameters and credentials
$authorization = "authorization"; // its value should just be your API Key

var lib = require('lib');
```

## Class Reference

### <a name="list_of_controllers"></a>List of Controllers

* [QueriesResourceController](#queries_resource_controller)
* [EventResourceController](#event_resource_controller)
* [ProjectRowResourceController](#project_row_resource_controller)
* [VersionsResourceController](#versions_resource_controller)
* [ProjectsResourceController](#projects_resource_controller)
* [DiscoveryResourceController](#discovery_resource_controller)
* [MaximumResourceController](#maximum_resource_controller)
* [MinimumResourceController](#minimum_resource_controller)
* [CountUniqueResourceController](#count_unique_resource_controller)
* [CountResourceController](#count_resource_controller)
* [EventCollectionResourceController](#event_collection_resource_controller)
* [PropertyResourceController](#property_resource_controller)
* [AverageResourceController](#average_resource_controller)
* [MedianResourceController](#median_resource_controller)
* [PercentileResourceController](#percentile_resource_controller)
* [SumResourceController](#sum_resource_controller)
* [SelectUniqueResourceController](#select_unique_resource_controller)
* [ExtractionResourceController](#extraction_resource_controller)
* [WardrobeResourceController](#wardrobe_resource_controller)
* [FunnelResourceController](#funnel_resource_controller)
* [SavedQueriesListResourceController](#saved_queries_list_resource_controller)
* [SavedQueryRowResourceController](#saved_query_row_resource_controller)
* [SavedQueryRowResultResourceController](#saved_query_row_result_resource_controller)

### <a name="queries_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".QueriesResourceController") QueriesResourceController

#### Get singleton instance

The singleton instance of the ``` QueriesResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.QueriesResourceController;
```

#### <a name="get_queries_resource"></a>![Method: ](https://apidocs.io/img/method.png ".QueriesResourceController.getQueriesResource") getQueriesResource

> GET returns the list of available queries and links to them.


```javascript
function getQueriesResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;

    controller.getQueriesResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="event_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EventResourceController") EventResourceController

#### Get singleton instance

The singleton instance of the ``` EventResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.EventResourceController;
```

#### <a name="get_event_resource"></a>![Method: ](https://apidocs.io/img/method.png ".EventResourceController.getEventResource") getEventResource

> GET returns schema information for all the event collections in this project, including properties and their type. It also returns links to sub-resources.


```javascript
function getEventResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;

    controller.getEventResource(input, function(error, response, context) {

    
	});
```



#### <a name="post_event_resource"></a>![Method: ](https://apidocs.io/img/method.png ".EventResourceController.postEventResource") postEventResource

> POST is for inserting multiple events in one or more collections, in a single request. See below for examples.


```javascript
function postEventResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| eventsBody |  ``` Required ```  | JSON arrays of events |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["eventsBody"] = {
        id : 21
    };

    controller.postEventResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="project_row_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ProjectRowResourceController") ProjectRowResourceController

#### Get singleton instance

The singleton instance of the ``` ProjectRowResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.ProjectRowResourceController;
```

#### <a name="get_project_row_resource"></a>![Method: ](https://apidocs.io/img/method.png ".ProjectRowResourceController.getProjectRowResource") getProjectRowResource

> GET returns detailed information about the specific project, as well as links to related resources


```javascript
function getProjectRowResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;

    controller.getProjectRowResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="versions_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".VersionsResourceController") VersionsResourceController

#### Get singleton instance

The singleton instance of the ``` VersionsResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.VersionsResourceController;
```

#### <a name="get_api_version"></a>![Method: ](https://apidocs.io/img/method.png ".VersionsResourceController.getAPIVersion") getAPIVersion

> Returns the available API versions. Please only use API version 3.0. Versions 1.0 and 2.0 have been deprecated.


```javascript
function getAPIVersion(callback)
```

#### Example Usage

```javascript


    controller.getAPIVersion(function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="projects_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ProjectsResourceController") ProjectsResourceController

#### Get singleton instance

The singleton instance of the ``` ProjectsResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.ProjectsResourceController;
```

#### <a name="get_projects_resource"></a>![Method: ](https://apidocs.io/img/method.png ".ProjectsResourceController.getProjectsResource") getProjectsResource

> Returns the projects accessible to the API user, as well as links to project sub-resources for discovery.


```javascript
function getProjectsResource(version, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var version = "version";

    controller.getProjectsResource(version, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="discovery_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".DiscoveryResourceController") DiscoveryResourceController

#### Get singleton instance

The singleton instance of the ``` DiscoveryResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.DiscoveryResourceController;
```

#### <a name="get_avaliable_child_project_resource"></a>![Method: ](https://apidocs.io/img/method.png ".DiscoveryResourceController.getAvaliableChildProjectResource") getAvaliableChildProjectResource

> Returns the available child resources. Currently, the only child resource is the Projects Resource.


```javascript
function getAvaliableChildProjectResource(version, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var version = "version";

    controller.getAvaliableChildProjectResource(version, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="maximum_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".MaximumResourceController") MaximumResourceController

#### Get singleton instance

The singleton instance of the ``` MaximumResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.MaximumResourceController;
```

#### <a name="get_maximum_resource"></a>![Method: ](https://apidocs.io/img/method.png ".MaximumResourceController.getMaximumResource") getMaximumResource

> returns the maximum numeric value for the target property in the event collection matching the given criteria. If strings and numbers are present, non-numeric values are ignored. The response will be a simple JSON object with one key: result, which maps to the numeric result described previously.


```javascript
function getMaximumResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| eventCollection |  ``` Optional ```  | The name of the event collection you are analyzing. |
| targetProperty |  ``` Optional ```  | The name of the property you are analyzing. |
| filters |  ``` Optional ```  | Filters are used to narrow down the events used in an analysis request based on event property values. |
| timeframe |  ``` Optional ```  | Similar to filters, a Timeframe is used to narrow down the events used in an analysis request based on the time that the event occurred. |
| interval |  ``` Optional ```  | An Interval specifies the size of time block to break a response into. This will cause a change in the response shape. |
| timezone |  ``` Optional ```  | Modifies the timeframe filters for Relative Timeframes to match a specific timezone. |
| groupBy |  ``` Optional ```  | The group_by parameter specifies the name of a property by which you would like to group the results. Using this parameter changes the response format. Read more about Group By to learn more. |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["eventCollection"] = event_collection;
        input["targetProperty"] = target_property;
        input["filters"] = "filters";
        input["timeframe"] = "timeframe";
        input["interval"] = "interval";
        input["timezone"] = "timezone";
        input["groupBy"] = group_by;

    controller.getMaximumResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="minimum_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".MinimumResourceController") MinimumResourceController

#### Get singleton instance

The singleton instance of the ``` MinimumResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.MinimumResourceController;
```

#### <a name="get_minimum_resource"></a>![Method: ](https://apidocs.io/img/method.png ".MinimumResourceController.getMinimumResource") getMinimumResource

> returns the minimum numeric value for the target property in the event collection matching the given criteria. If strings and numbers are present, non-numeric values are ignored. The response will be a simple JSON object with one key: result, which maps to the numeric result described previously.


```javascript
function getMinimumResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| eventCollection |  ``` Optional ```  | The name of the event collection you are analyzing. |
| targetProperty |  ``` Optional ```  | The name of the property you are analyzing. |
| filters |  ``` Optional ```  | Filters are used to narrow down the events used in an analysis request based on event property values. |
| timeframe |  ``` Optional ```  | Similar to filters, a Timeframe is used to narrow down the events used in an analysis request based on the time that the event occurred. |
| interval |  ``` Optional ```  | An Interval specifies the size of time block to break a response into. This will cause a change in the response shape |
| timezone |  ``` Optional ```  | Modifies the timeframe filters for Relative Timeframes to match a specific timezone. |
| groupBy |  ``` Optional ```  | The group_by parameter specifies the name of a property by which you would like to group the results. Using this parameter changes the response format. Read more about Group By to learn more. |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["eventCollection"] = event_collection;
        input["targetProperty"] = target_property;
        input["filters"] = "filters";
        input["timeframe"] = "timeframe";
        input["interval"] = "interval";
        input["timezone"] = "timezone";
        input["groupBy"] = group_by;

    controller.getMinimumResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="count_unique_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".CountUniqueResourceController") CountUniqueResourceController

#### Get singleton instance

The singleton instance of the ``` CountUniqueResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.CountUniqueResourceController;
```

#### <a name="get_count_unique_resource"></a>![Method: ](https://apidocs.io/img/method.png ".CountUniqueResourceController.getCountUniqueResource") getCountUniqueResource

>  returns the number of UNIQUE resources in the event collection matching the given criteria. The response will be a simple JSON object with one key: result, which maps to the numeric result described previously.


```javascript
function getCountUniqueResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| eventCollection |  ``` Required ```  | The name of the event collection you are analyzing. |
| targetProperty |  ``` Required ```  | The name of the property you are analyzing. |
| filters |  ``` Optional ```  | Filters are used to narrow down the events used in an analysis request based on event property values. |
| timeframe |  ``` Optional ```  | Similar to filters, a Timeframe is used to narrow down the events used in an analysis request based on the time that the event occurred. |
| interval |  ``` Optional ```  | An Interval specifies the size of time block to break a response into. This will cause a change in the response shape. |
| timezone |  ``` Optional ```  | Modifies the timeframe filters for Relative Timeframes to match a specific timezone. |
| groupBy |  ``` Optional ```  | he group_by parameter specifies the name of a property by which you would like to group the results. Using this parameter changes the response format |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["eventCollection"] = event_collection;
        input["targetProperty"] = target_property;
        input["filters"] = "filters";
        input["timeframe"] = "timeframe";
        input["interval"] = "interval";
        input["timezone"] = "timezone";
        input["groupBy"] = group_by;

    controller.getCountUniqueResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="count_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".CountResourceController") CountResourceController

#### Get singleton instance

The singleton instance of the ``` CountResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.CountResourceController;
```

#### <a name="get_count_resource"></a>![Method: ](https://apidocs.io/img/method.png ".CountResourceController.getCountResource") getCountResource

>  returns the number of resources in the event collection matching the given criteria. The response will be a simple JSON object with one key: a numeric result.


```javascript
function getCountResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| eventCollection |  ``` Required ```  | he name of the event collection you are analyzing. |
| filters |  ``` Optional ```  | Filters are used to narrow down the events used in an analysis request based on event property values. |
| timeframe |  ``` Optional ```  | Similar to filters, a Timeframe is used to narrow down the events used in an analysis request based on the time that the event occurred. |
| interval |  ``` Optional ```  | An Interval specifies the size of time block to break a response into. This will cause a change in the response shape. |
| timezone |  ``` Optional ```  | Modifies the timeframe filters for Relative Timeframes to match a specific timezone. |
| groupBy |  ``` Optional ```  | The group_by parameter specifies the name of a property by which you would like to group the results. Using this parameter changes the response format. Read more about Group By to learn more. |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["eventCollection"] = event_collection;
        input["filters"] = "filters";
        input["timeframe"] = "timeframe";
        input["interval"] = "interval";
        input["timezone"] = "timezone";
        input["groupBy"] = group_by;

    controller.getCountResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="event_collection_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".EventCollectionResourceController") EventCollectionResourceController

#### Get singleton instance

The singleton instance of the ``` EventCollectionResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.EventCollectionResourceController;
```

#### <a name="delete_event_collection_resource"></a>![Method: ](https://apidocs.io/img/method.png ".EventCollectionResourceController.deleteEventCollectionResource") deleteEventCollectionResource

> DELETE is for deleting the entire event collection. This is irreversible and will only work for collections under 10k events.


```javascript
function deleteEventCollectionResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| eventCollection |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["eventCollection"] = event_collection;

    controller.deleteEventCollectionResource(input, function(error, response, context) {

    
	});
```



#### <a name="get_event_collection_resource"></a>![Method: ](https://apidocs.io/img/method.png ".EventCollectionResourceController.getEventCollectionResource") getEventCollectionResource

> GET returns available schema information for this event collection, including properties and their type. It also returns links to sub-resources.


```javascript
function getEventCollectionResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| eventCollection |  ``` Required ```  | TODO: Add a parameter description |
| filters |  ``` Optional ```  | he filters to use when deleting events. See Filters for more information. |
| timeframe |  ``` Optional ```  | The timeframe to use when deleting events. See Timeframe for more information. |
| timezone |  ``` Optional ```  | The timezone to use when specifying a timeframe (while deleting events). See Timezone for more information. |
| data |  ``` Optional ```  | The event body you want to save to Keen IO, URL-encoded AND base-64 encoded |
| redirect |  ``` Optional ```  | The URL you want to redirect the user to after the event is saved. If you don?t include a protocol (http:// or https://), we?ll automatically add that for you. |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["eventCollection"] = event_collection;
        input["filters"] = "filters";
        input["timeframe"] = "timeframe";
        input["timezone"] = "timezone";
        input["data"] = "data";
        input["redirect"] = "redirect";

    controller.getEventCollectionResource(input, function(error, response, context) {

    
	});
```



#### <a name="post_event_collection_resource"></a>![Method: ](https://apidocs.io/img/method.png ".EventCollectionResourceController.postEventCollectionResource") postEventCollectionResource

> POST is for inserting one event at a time in a single request.


```javascript
function postEventCollectionResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| eventCollection |  ``` Required ```  | Single JSON event |
| eventBody |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["eventCollection"] = event_collection;
        input["eventBody"] = {
        id : 21
    };

    controller.postEventCollectionResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="property_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PropertyResourceController") PropertyResourceController

#### Get singleton instance

The singleton instance of the ``` PropertyResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.PropertyResourceController;
```

#### <a name="delete_property_resource"></a>![Method: ](https://apidocs.io/img/method.png ".PropertyResourceController.deletePropertyResource") deletePropertyResource

> DELETE is for removing a property and deleting all values stored with that property name.


```javascript
function deletePropertyResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| eventCollection |  ``` Required ```  | TODO: Add a parameter description |
| propertyName |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["eventCollection"] = event_collection;
        input["propertyName"] = property_name;

    controller.deletePropertyResource(input, function(error, response, context) {

    
	});
```



#### <a name="get_property_resource"></a>![Method: ](https://apidocs.io/img/method.png ".PropertyResourceController.getPropertyResource") getPropertyResource

> GET returns the property name, type, and a link to sub-resources


```javascript
function getPropertyResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| eventCollection |  ``` Required ```  | TODO: Add a parameter description |
| propertyName |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["eventCollection"] = event_collection;
        input["propertyName"] = property_name;

    controller.getPropertyResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="average_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".AverageResourceController") AverageResourceController

#### Get singleton instance

The singleton instance of the ``` AverageResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.AverageResourceController;
```

#### <a name="get_average_resource"></a>![Method: ](https://apidocs.io/img/method.png ".AverageResourceController.getAverageResource") getAverageResource

> returns the average across all numeric values for the target property in the event collection matching the given criteria. Non-numeric values are ignored. The response will be a simple JSON object with one key: result, which maps to the numeric result described previously. The response will be a simple JSON object with one key: result, which maps to the numeric result described previously.


```javascript
function getAverageResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| eventCollection |  ``` Required ```  | - The name of the event collection you are analyzing. |
| targetProperty |  ``` Required ```  | The name of the property you are analyzing. |
| interval |  ``` Required ```  | An Interval specifies the size of time block to break a response into. This will cause a change in the response shape. |
| filters |  ``` Optional ```  | Filters are used to narrow down the events used in an analysis request based on event property values. |
| timeframe |  ``` Optional ```  | Similar to filters, a Timeframe is used to narrow down the events used in an analysis request based on the time that the event occurred. |
| timezone |  ``` Optional ```  | Modifies the timeframe filters for Relative Timeframes to match a specific timezone. |
| groupBy |  ``` Optional ```  | The group_by parameter specifies the name of a property by which you would like to group the results. Using this parameter changes the response format. Read more about Group By to learn more. |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["eventCollection"] = event_collection;
        input["targetProperty"] = target_property;
        input["interval"] = "interval";
        input["filters"] = "filters";
        input["timeframe"] = "timeframe";
        input["timezone"] = "timezone";
        input["groupBy"] = group_by;

    controller.getAverageResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="median_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".MedianResourceController") MedianResourceController

#### Get singleton instance

The singleton instance of the ``` MedianResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.MedianResourceController;
```

#### <a name="get_median_resource"></a>![Method: ](https://apidocs.io/img/method.png ".MedianResourceController.getMedianResource") getMedianResource

> returns the median across all numeric values for the target property in the event collection matching the given criteria. Non-numeric values are ignored. The response will be a simple JSON object with one key: result, which maps to the numeric result described previously. The response will be a simple JSON object with one key: result, which maps to the numeric result described previously.


```javascript
function getMedianResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| eventCollection |  ``` Required ```  | The name of the event collection you are analyzing. |
| targetProperty |  ``` Required ```  | The name of the property you are analyzing. |
| version |  ``` Optional ```  | TODO: Add a parameter description |
| filters |  ``` Optional ```  | Filters are used to narrow down the events used in an analysis request based on event property values. |
| timeframe |  ``` Optional ```  | Similar to filters, a Timeframe is used to narrow down the events used in an analysis request based on the time that the event occurred. |
| interval |  ``` Optional ```  | An Interval specifies the size of time block to break a response into. This will cause a change in the response shape. |
| timezone |  ``` Optional ```  | Modifies the timeframe filters for Relative Timeframes to match a specific timezone. |
| groupBy |  ``` Optional ```  | The group_by parameter specifies the name of a property by which you would like to group the results. Using this parameter changes the response format. Read more about Group By to learn more. |



#### Example Usage

```javascript

    var input = [];
        input["projectId"] = project_id;
        input["eventCollection"] = event_collection;
        input["targetProperty"] = target_property;
        input["version"] = "version";
        input["filters"] = "filters";
        input["timeframe"] = "timeframe";
        input["interval"] = "interval";
        input["timezone"] = "timezone";
        input["groupBy"] = group_by;

    controller.getMedianResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="percentile_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".PercentileResourceController") PercentileResourceController

#### Get singleton instance

The singleton instance of the ``` PercentileResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.PercentileResourceController;
```

#### <a name="get_percentile_resource"></a>![Method: ](https://apidocs.io/img/method.png ".PercentileResourceController.getPercentileResource") getPercentileResource

>  returns the specified percentile across all numeric values for the target property in the event collection matching the given criteria. Non-numeric values are ignored. The response will be a simple JSON object with one key: result, which maps to the numeric result described previously. The response will be a simple JSON object with one key: result, which maps to the numeric result described previously.


```javascript
function getPercentileResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| eventCollection |  ``` Required ```  | The name of the event collection you are analyzing. |
| targetProperty |  ``` Required ```  | he name of the property you are analyzing. percentile (required) - The specific percentile you wish to calculate, supporting 0-100 with two decimal places of precision for example, 99.99 |
| filters |  ``` Optional ```  | Filters are used to narrow down the events used in an analysis request based on event property values. |
| timeframe |  ``` Optional ```  | imilar to filters, a Timeframe is used to narrow down the events used in an analysis request based on the time that the event occurred. |
| interval |  ``` Optional ```  | An Interval specifies the size of time block to break a response into. This will cause a change in the response shape. |
| timezone |  ``` Optional ```  | A Timezone modifies the timeframe filters for Relative Timeframes to match a specific timezone. |
| groupBy |  ``` Optional ```  | The Group By parameter specifies the name of a property by which you would like to group the results. Using this parameter changes the response format. |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["eventCollection"] = event_collection;
        input["targetProperty"] = target_property;
        input["filters"] = "filters";
        input["timeframe"] = "timeframe";
        input["interval"] = "interval";
        input["timezone"] = "timezone";
        input["groupBy"] = group_by;

    controller.getPercentileResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="sum_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SumResourceController") SumResourceController

#### Get singleton instance

The singleton instance of the ``` SumResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.SumResourceController;
```

#### <a name="get_sum_resource"></a>![Method: ](https://apidocs.io/img/method.png ".SumResourceController.getSumResource") getSumResource

> TODO: Add a method description


```javascript
function getSumResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| apiKey |  ``` Required ```  | Read Key for the project containing the data you are analyzing. See Authentication for more information |
| eventCollection |  ``` Required ```  | he name of the event collection you are analyzing. |
| targetProperty |  ``` Required ```  | The name of the property you are analyzing. |
| filters |  ``` Optional ```  | Filters are used to narrow down the events used in an analysis request based on event property values. |
| timeframe |  ``` Optional ```  | Similar to filters, a Timeframe is used to narrow down the events used in an analysis request based on the time that the event occurred. |
| interval |  ``` Optional ```  | An Interval specifies the size of time block to break a response into. This will cause a change in the response shape. |
| timezone |  ``` Optional ```  | Modifies the timeframe filters for Relative Timeframes to match a specific timezone. |
| groupBy |  ``` Optional ```  | The group_by parameter specifies the name of a property by which you would like to group the results. Using this parameter changes the response format. Read more about Group By to learn more. |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["apiKey"] = api_key;
        input["eventCollection"] = event_collection;
        input["targetProperty"] = target_property;
        input["filters"] = "filters";
        input["timeframe"] = "timeframe";
        input["interval"] = "interval";
        input["timezone"] = "timezone";
        input["groupBy"] = group_by;

    controller.getSumResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="select_unique_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SelectUniqueResourceController") SelectUniqueResourceController

#### Get singleton instance

The singleton instance of the ``` SelectUniqueResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.SelectUniqueResourceController;
```

#### <a name="get_select_unique_resource"></a>![Method: ](https://apidocs.io/img/method.png ".SelectUniqueResourceController.getSelectUniqueResource") getSelectUniqueResource

>  returns a list of UNIQUE resources in the event collection matching the given criteria. The response will be a simple JSON object with one key: result, which maps to an array of unique property values.


```javascript
function getSelectUniqueResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| eventCollection |  ``` Required ```  | The name of the event collection you are analyzing. |
| targetProperty |  ``` Required ```  | the name of the property you are analyzing. |
| filters |  ``` Optional ```  | Filters are used to narrow down the events used in an analysis request based on event property values. |
| timeframe |  ``` Optional ```  | Similar to filters, a Timeframe is used to narrow down the events used in an analysis request based on the time that the event occurred. |
| interval |  ``` Optional ```  | An Interval specifies the size of time block to break a response into. This will cause a change in the response shape. |
| timezone |  ``` Optional ```  | Modifies the timeframe filters for Relative Timeframes to match a specific timezone. |
| groupBy |  ``` Optional ```  | The group_by parameter specifies the name of a property by which you would like to group the results. Using this parameter changes the response format. Read more about Group By to learn more. |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["eventCollection"] = event_collection;
        input["targetProperty"] = target_property;
        input["filters"] = "filters";
        input["timeframe"] = "timeframe";
        input["interval"] = "interval";
        input["timezone"] = "timezone";
        input["groupBy"] = group_by;

    controller.getSelectUniqueResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="extraction_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".ExtractionResourceController") ExtractionResourceController

#### Get singleton instance

The singleton instance of the ``` ExtractionResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.ExtractionResourceController;
```

#### <a name="get_extraction_resource"></a>![Method: ](https://apidocs.io/img/method.png ".ExtractionResourceController.getExtractionResource") getExtractionResource

> creates an extraction request for full-form event data with all property values. See Data Extractions for more details. If the query string parameter email is specified, then the extraction will be processed asynchronously and an e-mail will be sent to the specified address when it completes. The email will include a link to a downloadable CSV file. If email is omitted, then the extraction will be processed in-line and JSON results will be returned in the GET request.


```javascript
function getExtractionResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| eventCollection |  ``` Required ```  | The name of the event collection you are analyzing. |
| filters |  ``` Optional ```  | Filters are used to narrow down the events used in an analysis request based on event property values. |
| timeframe |  ``` Optional ```  | A Timeframe specifies the events to use for analysis based on a window of time. |
| email |  ``` Optional ```  | If an email address is specified, an email will be sent to it when your extraction is ready for download. If email is not specified, your extraction will be processed synchronously and your data will be returned as JSON. |
| latest |  ``` Optional ```  | An integer containing the number of most recent events to extract. |
| propertyNames |  ``` Optional ```  | A URL-encoded array of strings containing properties you wish to extract. If this parameter is omitted, all properties will be returned. |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["eventCollection"] = event_collection;
        input["filters"] = "filters";
        input["timeframe"] = "timeframe";
        input["email"] = "email";
        input["latest"] = 171;
        input["propertyNames"] = property_names;

    controller.getExtractionResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="wardrobe_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".WardrobeResourceController") WardrobeResourceController

#### Get singleton instance

The singleton instance of the ``` WardrobeResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.WardrobeResourceController;
```

#### <a name="post_wardrobe_resource"></a>![Method: ](https://apidocs.io/img/method.png ".WardrobeResourceController.postWardrobeResource") postWardrobeResource

> Use this resource to request a garment of a given size to a given address. This is really just the Event Collect Resource, except you must use a specific project ID, write key, and collection name. See below. POST is for inserting one event at a time in a single request, for a single person. Examples below. Note: Wardrobe resource has questionable availability and response time depending on inventory, expense to ship to your country, trolls, team temperament, and our willingness to visit the post office in a given week.


```javascript
function postWardrobeResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| body |  ``` Required ```  | Single JSON event |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["body"] = {
        id : 21
    };

    controller.postWardrobeResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="funnel_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".FunnelResourceController") FunnelResourceController

#### Get singleton instance

The singleton instance of the ``` FunnelResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.FunnelResourceController;
```

#### <a name="get_funnel_resource"></a>![Method: ](https://apidocs.io/img/method.png ".FunnelResourceController.getFunnelResource") getFunnelResource

>  Funnels count relevant events in succession. See Funnels for more details!


```javascript
function getFunnelResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| steps |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["steps"] = "steps";

    controller.getFunnelResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="saved_queries_list_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SavedQueriesListResourceController") SavedQueriesListResourceController

#### Get singleton instance

The singleton instance of the ``` SavedQueriesListResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.SavedQueriesListResourceController;
```

#### <a name="get_saved_queries_list_resource"></a>![Method: ](https://apidocs.io/img/method.png ".SavedQueriesListResourceController.getSavedQueriesListResource") getSavedQueriesListResource

> GET returns all the available Saved Queries for the specified project as well as links to child-resources.


```javascript
function getSavedQueriesListResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;

    controller.getSavedQueriesListResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="saved_query_row_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SavedQueryRowResourceController") SavedQueryRowResourceController

#### Get singleton instance

The singleton instance of the ``` SavedQueryRowResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.SavedQueryRowResourceController;
```

#### <a name="get_saved_query_row_resource"></a>![Method: ](https://apidocs.io/img/method.png ".SavedQueryRowResourceController.getSavedQueryRowResource") getSavedQueryRowResource

> GET returns information about the specified Saved Query and includes links to child-resources.


```javascript
function getSavedQueryRowResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| savedQueryName |  ``` Required ```  | TODO: Add a parameter description |
| analysisType |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["savedQueryName"] = saved_query_name;
        input["analysisType"] = analysis_type;

    controller.getSavedQueryRowResource(input, function(error, response, context) {

    
	});
```



#### <a name="put_saved_query_row_resource"></a>![Method: ](https://apidocs.io/img/method.png ".SavedQueryRowResourceController.putSavedQueryRowResource") putSavedQueryRowResource

> PUT either inserts a new Saved Query if it doesn?t already exist, or updates an existing Saved Query if it does exist.


```javascript
function putSavedQueryRowResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| savedQueryName |  ``` Required ```  | TODO: Add a parameter description |
| analysisType |  ``` Required ```  | TODO: Add a parameter description |
| body |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["savedQueryName"] = saved_query_name;
        input["analysisType"] = analysis_type;
        input["body"] = {
        id : 21
    };

    controller.putSavedQueryRowResource(input, function(error, response, context) {

    
	});
```



#### <a name="delete_saved_query_row_resource"></a>![Method: ](https://apidocs.io/img/method.png ".SavedQueryRowResourceController.deleteSavedQueryRowResource") deleteSavedQueryRowResource

> DELETE just plain old deletes the Saved Query.


```javascript
function deleteSavedQueryRowResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| savedQueryName |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["savedQueryName"] = saved_query_name;

    controller.deleteSavedQueryRowResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)

### <a name="saved_query_row_result_resource_controller"></a>![Class: ](https://apidocs.io/img/class.png ".SavedQueryRowResultResourceController") SavedQueryRowResultResourceController

#### Get singleton instance

The singleton instance of the ``` SavedQueryRowResultResourceController ``` class can be accessed from the API Client.

```javascript
var controller = lib.SavedQueryRowResultResourceController;
```

#### <a name="get_saved_query_row_result_resource"></a>![Method: ](https://apidocs.io/img/method.png ".SavedQueryRowResultResourceController.getSavedQueryRowResultResource") getSavedQueryRowResultResource

> GET returns the results of the specified Saved Query.


```javascript
function getSavedQueryRowResultResource(input, callback)
```
#### Parameters

| Parameter | Tags | Description |
|-----------|------|-------------|
| version |  ``` Required ```  | TODO: Add a parameter description |
| projectId |  ``` Required ```  | TODO: Add a parameter description |
| savedQueryName |  ``` Required ```  | TODO: Add a parameter description |



#### Example Usage

```javascript

    var input = [];
        input["version"] = "version";
        input["projectId"] = project_id;
        input["savedQueryName"] = saved_query_name;

    controller.getSavedQueryRowResultResource(input, function(error, response, context) {

    
	});
```



[Back to List of Controllers](#list_of_controllers)



