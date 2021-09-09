# create-new-revealjs-template

Reveal.js template presentation as a GitHub repo Template

* Includes Reveal.js as a Git submodule so that its commit history is not confused with this presentation's history
* Makes future updating of Reveal.js version very easy
* Reduces the size of the presentation repositories significantly

## Usage

1. Click 'Use This Template'
1. Name your presentation and it will be created in your own GitHub account/org
1. Customise as necessary
1. If you clone the repo locally you also need to get the submodule files with `git submodule update --init --recursive`
1. Push completed slides back to GitHub
1. Configure your GitHub pages settings to serve the slides from _youraccount_.github.io/_repositoryname_ (or custom domain even)
1. **Amaze your friends** by being able to share the URL of your live, interactive slides with your audience immediately. No more emailing PowerPoint attachments for YOU!

## Updating Reveal.js

* You may get Dependabot alerts from GitHub to warn you of vulnerabilities in the Reveal.js code. To make these go away, update the submodule.
* Use the command `git submodule update --rebase --remote` in the **root** of the repository (not the submodule directory) to update.
* link for info on updating submodules https://stackoverflow.com/questions/1979167/git-submodule-update

## Credits

* [Hakim El-Hattab](https://twitter.com/hakimel) for the simple awesome [Reveal.js](https://github.com/hakimel/reveal.js)
* [Martino Mensio](https://twitter.com/MartinoMensio) for his guide on how to use Reveal.js as a Git submodule in [this](https://martinomensio.medium.com/how-to-host-reveal-js-slides-on-github-pages-and-have-a-tidy-repository-1a363944c38d) blog post (and in doing so I learned how to use and not fear the Submodule!)
* [Excalidraw](https://excalidraw.com/) which is a separate project, mentioned in my presentation template, but I love it so much I wanted to plug it here too.

## License

* MIT Licensed as per Reveal.js itself

## Contributing

* Feel free to make suggestions and PRs to the template repo
