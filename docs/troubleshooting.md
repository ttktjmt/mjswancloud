# Troubleshooting

## A simulation does not load

Start with the message on the page.

### "This simulation is not available."

The simulation was built with an mjswan release that mjswan Cloud no longer runs. Your browser is not the problem.

- **If it is your simulation,** sign in, open its page, and click **Choose a newer engine**. The link, views, likes, and comments stay as they are, so there is no need to upload it again.
- **If it belongs to someone else,** only its author can fix it. You can let them know in the comments.

### "This simulation could not be loaded. Its data files may be unavailable."

The page could not download the simulation's files.

- Reload the page. An interrupted connection is the most common cause.
- Check whether an ad or privacy blocker is blocking `mjswanusercontent.com`. Simulations and their files are served from there.
- If it keeps happening, [open a bug report](https://github.com/ttktjmt/mjswancloud/issues/new?template=bug_report.yml) with the link to the simulation.

### A different message appears

The message comes from the engine that draws the scene.

- Try another browser, or update the one you use.
- Check that hardware acceleration is turned on in your browser settings. The engine needs WebGL.
- If the message stays, [open a bug report](https://github.com/ttktjmt/mjswancloud/issues/new?template=bug_report.yml) and copy the message into it exactly.

### Nothing appears, and there is no message

- A large scene can take a while to download the first time. Give it a minute.
- Check that WebGL works in your browser at [get.webgl.org](https://get.webgl.org).
- Open the browser console (F12, then the Console tab) and include what it shows in a [bug report](https://github.com/ttktjmt/mjswancloud/issues/new?template=bug_report.yml).

## A publish is refused

`mjswan publish` and the upload page both say why a build was refused. Most messages say what to do; these two need more context:

| Message | What to do |
|---|---|
| `Unsupported engine version: …` | The build was made with an mjswan release that mjswan Cloud does not run. If your mjswan is old, update it with `pip install -U mjswan`, rebuild, and publish again. If it is a very new release, support may not be added yet: [ask in Discussions](https://github.com/ttktjmt/mjswancloud/discussions/categories/q-a). |
| `This build uses custom-TS MDP terms …` | mjswan Cloud never runs code from a build, so a build with author-written TypeScript terms cannot be published. Traced ONNX terms are fine. |

A license file can also stop a publish, when its terms do not allow redistribution. The message names the file: remove that asset, or use one whose license allows sharing.

Size, file count, file type, and account limits are listed under "Service limits" in the [Terms](https://mjswan.com/terms).

For anything else, [open a bug report](https://github.com/ttktjmt/mjswancloud/issues/new?template=bug_report.yml) and include the full output.

## Publishing, likes, or views stop working

The beta runs on daily usage allowances. When one runs out, publishing, likes, and view counts can stop until it resets; published simulations stay viewable. Try again later.
