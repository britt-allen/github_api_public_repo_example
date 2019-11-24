# Listing my public GitHub repos


I wrote code to list my public GitHub repositories leveraging the [Requests library](https://pypi.org/project/requests/2.7.0/) and [GitHub's API](https://developer.github.com/v3/repos/#list-your-repositories).

By default, when you access the API as an un-authenthicated user you'll only be able to access public repos. I chose to go this route to avoid pushing up a notebook with private information (i.e my password or access token). I also created a private repo (picture below) to test this assumption. When you run my [code](https://github.com/traintestbritt/github_api_public_repo_example/blob/master/github_api_public_repo_example.ipynb) you'll see that this assumption holds true.

![GitHub Repo Screenshot](/github_repo_screenshot.png)

Although I've fully commented out my notebook I'll include instructions on how to run my code here:

- Download the [file](https://github.com/traintestbritt/github_api_public_repo_example/blob/master/github_api_public_repo_example.ipynb)
- Run the code in your application of choice
- You can expect the code to:
  - Import the Requests library
  - Create a resonse object with the results of an request to the GitHub API
  - Convert that response object to JSON
  - Print out the contents of the new JSON object
  - Print out all of the users repos by looping through the length of the JSON object
  - Print out additional and potentially helpful information about where the repos originated and how many there are
  
  * Please note that at the time of running this code I had 9 repos, of which 8 were accessible by the Github API
