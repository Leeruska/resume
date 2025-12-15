
The easy way to host your resume is by making a `resume.json` on gist.github.com. 

My gist: https://gist.github.com/Leeruska/da1e8dfb4793f28d5321e43913730580 which then automatically gets hosted at ___ 

You can just edit your Gist using the online GUI and it should update within less than a minute. 

## But

If you would like to have your `resume.json` in a repository aka like this, you can follow instructions by https://github.com/thomasdavis/resume.

You can set up a Github Action that automatically updates your gist `resume.json` to match what is in your repo everytime you push. 

If you checkout the `.github/workflows/gist.yml` file you should be able to figure it out with relative ease. Or feel free to ping me an issue. 

### TO-DO:
1) Create a gist called `resume.json` - DONE
2) Create or fork this repo and commit your updated `resume.json` - DONE
3) Create a Personal Github token that has just the `gist` scope 
4) Go to your repository settings, then to the secrets page, and add a new secret called `TOKEN` with the value being from the token you created in 3) - DONE
5) Now simply push to your repo, and your `resume.json` from the repo, will publish and override your gist `resume.json` and thus updating the registry to match
