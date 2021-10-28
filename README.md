# How to host Swagger API documentation with GitHub Pages

1. This respository is based on peterevans's blog: https://peterevans.dev/posts/how-to-host-swagger-docs-with-github-pages/
2. Clone this repo.
3. Update the `swagger.json` file you wish to host.
4. Ensure to have following in the swagger file. 

```
  "host": "cors-anywhere.herokuapp.com",
  "basePath": "/<your instance url>",
```
5. Publish the repo using github pages. Details mentioned below.
    - Go to the settings for your repository at `https://github.com/{github-username}/{repository-name}/settings` and enable GitHub Pages.

    ![Headers](/screenshots/swagger-github-pages.png?raw=true)
    
6. Browse to the Swagger documentation at `https://{github-username}.github.io/{repository-name}/`.

7. For present repo swagger file is: https://priyankajayaswal1.github.io/swagger-ui-for-dummy-service/

8. For first time on making a request you might get 403. This is because you'd need to request for temporary access on the request url. 
 - Go to the request uri as shown below and click on the "Request temporary access to the demo server" button, to temporarily restore the full functionality of CORS Anywhere for your client only.
![Headers](/screenshots/request-uri-for-cors.png?raw=true)


9. Relevant reference to enable cors: https://github.com/Rob--W/cors-anywhere/issues/301