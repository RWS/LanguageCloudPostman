# Language Cloud APIs for Postman

A [Postman](https://www.postman.com/) collection for quick and easy usage of our [RESTful APIs](https://languagecloud.sdl.com/lc/api-docs/). 

## Installation

You can download the Postman collection from [here](https://github.com/sdl/language-cloud-public-api-postman/blob/develop/postmanCollection.json?raw=true).

Either copy the collection url from above, save it as a json file on your computer or copy the entirety of the file content and import it into Postman.

![image](https://user-images.githubusercontent.com/10993097/118100979-c343a000-b3df-11eb-9a1c-e404f662b269.png)

## Configuration

The imported collection is already set up for you to get started as fast as possible. 
We make use of collection level variables and an inherited authentication mechanism.

For exaple, the authentication is already set up to use the Bearer Token scheme and will use the token value provided by `{{lc-access-token}}` variable. This token is being populated with the correct value each time you `Obtain a client credentials access token`, via the Tests tab.

One thing you need to do before proceeding is to fill in the `{{lc_tenant}}` variable with your own tenant id. Prepend the id with LC- so the final value looks like `LC-00000000000000000`

Don't forget to save the collection!

![image](https://user-images.githubusercontent.com/10993097/130009444-9dc0e314-7763-46aa-ad8d-20cfda3510de.png)


### Authentication
To start working with the Language Cloud API, you first need to authenticate. 

You can find the authentication call under the `Authorization (Start Here)` folder. Fill in your `client_id` and `client_secret` and perform the request.

If the authentication is successful, the token will be extracted automatically from the response and saved to the `{{lc-access-token}}` variable.

![image](https://user-images.githubusercontent.com/10993097/118103532-b1173100-b3e2-11eb-97c0-92df2f3794ec.png)

### Usage

After you have authenticated successfully, you can start interacting with the Language Cloud API.

For example, we can get information about a project by using the **GetProject** request from the **Project** folder.

Simply fill in your `projectId` and click SEND. Optionally, you can supply values to the `fields` paramater to recieve only data that is of interrest.

![image](https://user-images.githubusercontent.com/10993097/118110695-68b04100-b3eb-11eb-8356-5bd6e21185c8.png)


