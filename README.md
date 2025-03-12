# My resume  made with JSON resume.

Info on JSOM rsume can be found here: https://jsonresume.org/getting-started


For example mine can be found at https://gist.github.com/Leeruska/1c9dfde0c1ffcbf0fe17b35adbf34767 which then automatically gets hosted at https://registry.jsonresume.org/thomasdavis 

You can just edit your Gist using the online GUI and it should update within less than a minute. 

## But

I wanted to have my `resume.json` in a repository.

I will set up a Github Action that automatically updates my gist `resume.json` to match what is in my repo on every push. 

Workflow is on the `.github/workflows/gist.yml` file.

The basic steps are

1) Create a gist called `resume.json` 
2) Create or fork this repo and commit your updated `resume.json` 
3) Create a Personal Github token that has just the `gist` scope 
4) Go to your repository settings, then to the secrets page, and add a new secret called `TOKEN` with the value being from the token you created in 3) 
5) Now simply push to your repo, and your `resume.json` from the repo, will publish and override your gist `resume.json` and thus updating the registry to match
