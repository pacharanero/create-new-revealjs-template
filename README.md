# create-new-revealjs-template

Create a new [Reveal.js](https://github.com/hakimel/reveal.js) presentation from this GitHub Template repository.

* Includes Reveal.js as a **Git submodule** so that Reveal.js's Git commit history is not confused with the presentation's Git commit history.
* The default presentation uses inline Markdown for the slide content, but you can use HTML or a mix of both. I've included a few examples of how to use fragment transitions in Markdown in the example slides.
* Makes future updating of Reveal.js version very easy (see [Updating](#updating-revealjs) below).
* Reduces the size of the presentation repositories significantly.
* Automatically creates update PRs via Dependabot (experimental).
* Scripts included in the `s/` directory for serving the presentation locally, updating the submodule manually, and for creating a PDF version of the slides.


## Usage

1. Click the 'Use This Template' button.

1. Name your presentation repository and it will be created in your own GitHub account/org.

1. Customise as necessary, by cloning locally (or even just using the Github editing UI). See the [Reveal.js documentation](https://revealjs.com/markup/) for information on how to get started with Reveal.js, how to add features, and customise your presentations as necessary.

1. If you clone the repo locally you also need to get the submodule files with `git submodule update --init --recursive`

1. You can use any local server to serve the files. One option is `live-server` which you can install and use with the `s/serve` script. You can also manually install and run it with `npm install -g live-server` then type `live-server` in the command line. Using a local server gives you additional features such as live-reload and some of the more advanced [Reveal.js](https://github.com/hakimel/reveal.js) features.

1. Push completed slides back to GitHub

1. Configure your GitHub pages settings to serve the slides from _youraccount_.github.io/_repositoryname_ (or custom domain even)

1. **Amaze your friends** (and blow the minds of the AV team at conferences) by presenting from a web browser and being able to share the URL of your live, interactive slides with your audience immediately. No more emailing PowerPoint attachments for YOU!


## Updating Reveal.js

* You may get Dependabot alerts from GitHub to warn you of vulnerabilities in the Reveal.js code. I have included a GitHub Action that will automatically merge Dependabot's PR to update the Reveal.js submodule. For security reasons this Actions is not trusted by GitHub when you make your own repository from this template, so you will need to enable it in the Actions tab of your repository.

* To update you can use the script `s/update` which updates Reveal.js to latest. The first time you run this command (on some systems) you will need to make it executable, by running `chmod +x s/update`. This can also be done in the File Manager UI in many systems.

* For older repositories made from this template, the command to run is `git submodule update --rebase --remote`, from the **root** of the repository (not the reveal.js submodule directory itself) to update.

* link for info on updating submodules https://stackoverflow.com/questions/1979167/git-submodule-update


## PDF export of slides

* You can export your slides to PDF using the script `s/pdf`. This will create a PDF file in the root of the repository with the name `slides.pdf`.


## Credits

* [Hakim El-Hattab](https://twitter.com/hakimel) for the simply awesome [Reveal.js](https://github.com/hakimel/reveal.js)
* [Martino Mensio](https://twitter.com/MartinoMensio) for his guide on how to use Reveal.js as a Git submodule in [this](https://martinomensio.medium.com/how-to-host-reveal-js-slides-on-github-pages-and-have-a-tidy-repository-1a363944c38d) blog post (and in doing so I learned how to use and not fear the Submodule!)
* [Excalidraw](https://excalidraw.com/) which is a separate project, mentioned in my presentation template, but I love it so much I wanted to plug it here too.

## License

* MIT Licensed as per Reveal.js itself

## Contributing

* Feel free to make suggestions and PRs to the template repo
