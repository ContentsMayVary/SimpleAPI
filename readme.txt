This solution is for the YouTube tutorial: https://www.youtube.com/watch?v=SOtC1VLZKm4
Also see https://dotnetplaybook.com/build-test-and-deploy-a-rest-api-with-azure-devops/

In it's entirety, this supports the following scenario:

(1) Edit local code.
(2) Push changes to GitHub.
(3) Build pipeline automatically runs.
(4) Release pipeline automatically runs.
(5) Now you can access https://matthewwatson.azurewebsites.net/ and the website now contains the changes.

----
URLS
----

Deployment Web Site: https://matthewwatson.azurewebsites.net/
Test like so: https://matthewwatson.azurewebsites.net/api/simple/420 -> Should display "420" in the browser.
Azure DevOps: https://dev.azure.com/Grimfane (this is where you set up the release pipelines)
Azure Services: https://portal.azure.com/ (this is where you set up the Web Site resource)

---------
GIT notes
---------

After changing code:

git add .
git commit -m "Comment for the changes"
git push origin master
