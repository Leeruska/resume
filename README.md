# JSON Resume

## What and Why

I wanted to test Github Actions, gist and json with this small "JSON Resume" project. The idea started from jsonresume.org where I got the ideas, examples and help to do this.

At the same time I get to have a new Resume/CV and easile change the theme when needed.

## How

*Original instructions from https://github.com/thomasdavis/resume.*

The easy way to host your resume is by making a `resume.json` on gist.github.com. 

My gist is here https://gist.github.com/Leeruska/da1e8dfb4793f28d5321e43913730580 which then automatically gets hosted at https://registry.jsonresume.org/Leeruska.

You *can* just edit your Gist using the online GUI and it should update within less than a minute. **But** if you would like to have your `resume.json` in a repository aka like this, you can follow instructions by https://github.com/thomasdavis/resume.

You can set up a Github Action that automatically updates your gist `resume.json` to match what is in your repo everytime you push. 

If you checkout the `.github/workflows/gist.yml` file you should be able to figure it out with relative ease. 

### TO-DO:
1) Create a gist called `resume.json` - DONE
2) Create or fork from the  repo and commit your updated `resume.json` - DONE
3) Create a Personal Github token that has just the `gist` scope - DONE
4) Go to your repository settings, then to the secrets page, and add a new secret called `TOKEN` with the value being from the token you created in 3) - DONE
5) Now simply push to your repo, and your `resume.json` from the repo, will publish and override your gist `resume.json` and thus updating the registry to match - DONE!

## Personal notes

- Gist
  - had to google what/where/how, hadn't use that before.
- GitHub branching and pull requests
  - I did not realize that GIthub put the original repository that I forked as the main when I was making a pull request. So that was foolish of me. :')
- The automatic update from gist to jsonresume.org
  - this did not work because my json file was not valid. I needed a separate checker to realize that.
- Email address
  - I didn't want to put my real email address yet to the json-file, but it has to have somekind of email address to be valid json file. After fixing that it seems to work. For now. :)

-Leeruska-
