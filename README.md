# [CNG Education Working Group meeting notes](https://cng-education.github.io/meeting-notes/)

## Contributing

This is a [Quarto](https://quarto.org) project.
The development environment is managed by [Pixi](https://pixi.sh).


### Start a local preview server

```bash
pixi run preview
```

This will start a local preview server.
View your changes immediately in your browser!
Any changes to the website content will trigger an automatic re-render.


### Render the website

```bash
pixi run render
```

This will build the website for deployment.
If you're developing locally, don't worry about this -- it occurs in our CD pipeline.


## Common activities

### Initialize and sync meeting notes

Initialize meeting notes on HackMD by navigating to the "Actions" tab of this repo.
Then select "Setup / sync meeting notes" on the left panel.
Now click "Run workflow" in the main workflow listing panel.
Finally, fill in the date, and click "Run workflow".

<details>
  <summary>Screenshot</summary>
  <img src="https://github.com/user-attachments/assets/db567500-48ee-4e32-8cf3-5eab01cce96c">
</details>

A Pull Request and HackMD document will be created.
Visit the new PR to find the HackMD link.

When you're ready to sync data from HackMD back to GitHub, comment in the PR with `/bot please sync notes`.
See [PR #32](https://github.com/geojupyter/geojupyter.org/pull/32) for an example.

> [!NOTE]
> This job may occasionally fail with e.g. 403 response from HackMD.
> In the past, re-running the job has worked.
