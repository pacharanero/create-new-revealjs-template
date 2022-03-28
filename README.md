# create-new-revealjs-template

Reveal.js template presentation as a GitHub repo Template

* Includes Reveal.js as a Git submodule so that its commit history is not confused with this presentation's history
* Makes future updating of Reveal.js version very easy
* Reduces the size of the presentation repositories significantly

## Usage

1. Click 'Use This Template'

1. Name your presentation and it will be created in your own GitHub account/org

1. Customise as necessary, by cloning locally (or even just using the Github editing UI)

1. If you clone the repo locally you also need to get the submodule files with `git submodule update --init --recursive`

1. You can use any local server to serve the files. One option is live-server (install it with `npm install -g live-server' then type `live-server` in the command line). Using a local server gives you additional features such as live-reload and some of the more advanced Reveal.js features.

1. Push completed slides back to GitHub

1. Configure your GitHub pages settings to serve the slides from _youraccount_.github.io/_repositoryname_ (or custom domain even)

1. **Amaze your friends** by being able to share the URL of your live, interactive slides with your audience immediately. No more emailing PowerPoint attachments for YOU!

## Updating Reveal.js

* You may get Dependabot alerts from GitHub to warn you of vulnerabilities in the Reveal.js code. To make these go away, update the submodule.

* To update you can use the script `s/update` which updates Reveal.js to latest. The first time you run this command (on some systems) you will need to make it executable, by running `chmod +x s/update`. This can also be done in the File Manager UI in many systems.

* For older repositories made from this template, the command to run is `git submodule update --rebase --remote`, from the **root** of the repository (not the reveal.js submodule directory itself) to update.
* 
* link for info on updating submodules https://stackoverflow.com/questions/1979167/git-submodule-update

## Credits

* [Hakim El-Hattab](https://twitter.com/hakimel) for the simply awesome [Reveal.js](https://github.com/hakimel/reveal.js)
* [Martino Mensio](https://twitter.com/MartinoMensio) for his guide on how to use Reveal.js as a Git submodule in [this](https://martinomensio.medium.com/how-to-host-reveal-js-slides-on-github-pages-and-have-a-tidy-repository-1a363944c38d) blog post (and in doing so I learned how to use and not fear the Submodule!)
* [Excalidraw](https://excalidraw.com/) which is a separate project, mentioned in my presentation template, but I love it so much I wanted to plug it here too.

## License

* MIT Licensed as per Reveal.js itself

## Contributing

* Feel free to make suggestions and PRs to the template repo
