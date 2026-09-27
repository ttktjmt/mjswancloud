<p align="center">
  <img src="assets/logo.svg" alt="" width="96">
</p>

<h1 align="center">mjswan Cloud</h1>

<p align="center">
  <strong>Host, discover, and share interactive simulations built with <a href="https://github.com/ttktjmt/mjswan">mjswan</a>.</strong>
</p>

<p align="center">
  <a href="https://mjswan.com"><img src="https://img.shields.io/badge/website-mjswan.com-0284c7" alt="Website: mjswan.com"></a>
  <img src="https://img.shields.io/badge/status-open%20beta-e8a33d" alt="Status: open beta">
</p>


## Where to go

| I want to | Go to |
|---|---|
| Report something that is broken | [Troubleshooting](docs/troubleshooting.md) first, then [a bug report](https://github.com/ttktjmt/mjswancloud/issues/new?template=bug_report.yml) |
| Check for outages and changes | [Discussions: Announcements](https://github.com/ttktjmt/mjswancloud/discussions/categories/announcements) |
| Ask how something works | [Discussions: Q&A](https://github.com/ttktjmt/mjswancloud/discussions/categories/q-a) |
| Suggest a feature | [Discussions: Ideas](https://github.com/ttktjmt/mjswancloud/discussions/categories/ideas) |
| Report a security vulnerability | [Report it privately](https://github.com/ttktjmt/mjswancloud/security/advisories/new), not in a public issue |
| Report a simulation that infringes copyright | [dmca@mjswan.com](mailto:dmca@mjswan.com), as described in the [Terms](https://mjswan.com/terms) |
| Report a simulation that breaks the Terms in another way | [legal@mjswan.com](mailto:legal@mjswan.com) |
| Access, correct, or delete your personal data | [privacy@mjswan.com](mailto:privacy@mjswan.com), see the [Privacy Policy](https://mjswan.com/privacy) |


## What is mjswan Cloud?

Build a simulation with mjswan, publish it, and get a page you can share and embed on your own site. The simulation runs in the viewer's browser.

Only the data files of a build are uploaded, such as the scene, the policies, and license files. mjswan Cloud renders them with its own copy of the engine and never runs code from a build.

This repository is where mjswan Cloud collects **bug reports, questions, and feedback**.


## Publish a simulation

```bash
pip install mjswan
python build.py    # your build script; writes dist/
mjswan publish path/to/dist --title "My simulation"
```

The first `mjswan publish` signs you in with GitHub and prints the URL of the new page. You can also upload a `dist/` folder at [mjswan.com/upload](https://mjswan.com/upload).

More in the mjswan docs: [Publishing to mjswan Cloud](https://mjswan.readthedocs.io/en/latest/guides/publishing/) and [Embedding](https://mjswan.readthedocs.io/en/latest/guides/embedding/).


## Status

mjswan Cloud is in open beta, so features and limits may change. Every report is read; replies are best effort.


## Links

- [mjswan Cloud](https://mjswan.com): the platform
- [mjswan](https://github.com/ttktjmt/mjswan): the simulation framework
- [mjswan Playground](https://github.com/ttktjmt/mjswan_playground): demos built with mjswan
- [Terms of Service](https://mjswan.com/terms) and [Privacy Policy](https://mjswan.com/privacy)
