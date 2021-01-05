<p align="center">
  <img src="images/logo.png" alt="Rooibos test framework" width="200" height="200"/>
</p>
<h3 align="center">
Simple, mocha-inspired, flexible, fun Brightscript test framework for ROKU apps
</h3>
<p align="center">
  <img src="images/exampleImage.png" alt="Mocha test framework" />
</p>

[![Build Status](https://travis-ci.org/georgejecook/rooibos.svg?branch=master)](https://travis-ci.org/georgejecook/rooibos)
[![GitHub](https://img.shields.io/github/release/georgejecook/rooibos.svg?style=flat-square)](https://github.com/georgejecook/rooibos/releases) 

## Links
 - **[Documentation](docs/index.md)**
 - **[API Documentaiton](https://georgejecook.github.io/rooibos)**
 - **[CHANGELOG](CHANGELOG.md)**
 - **[VSCode snippets](docs/vsCodeSnippets.md)**
 - [Roku dev forum topic](https://forums.roku.com/viewforum.php?f=34)
 - \#roku channel on the [roku developer's slack](https://join.slack.com/t/rokudevelopers/shared_invite/enQtMzgyODg0ODY0NDM5LTc2ZDdhZWI2MDBmYjcwYTk5MmE1MTYwMTA2NGVjZmJiNWM4ZWY2MjY1MDY0MmViNmQ1ZWRmMWUzYTVhNzJiY2M)
 - [Issue tracker](https://github.com/georgejecook/rooibos/issues)
 - [Roadmap](ROADMAP.md)

## Development

Rooibos is an independent open-source project, maintained exclusively by volunteers.

You might want to help! Get in touch via the slack group, or raise issues.

## Thanks

Rooibos was hacked together from the official roku unit testing framework. I'd like to say a big thank you to the guys at roku who gave me permission to build upon their work. The original framework can be found here : [https://github.com/rokudev/unit-testing-framework](https://github.com/rokudev/unit-testing-framework)

Also thanks to the guys who made and maintain [mochaJs](https://mochajs.org/), on which many of my changes are based upon, as well as the structure of the documentation.

## FAQ
### Is Rooibos ready for production use?

Rooibos is the test framework used by several of my clients, running CI with over 3000 tests between them. It started life as rewrite of the official roku unit testing framework, which has been in circulation for several years.


### Is Rooibos actively maintained?

I am actively invovled in Rooibos's development, and add more features and fixes on a weekly basis. You can expect rapid responses to issues.

### Why did you not just merge back your changes to roku's unit testing framework

1. It does rewrite quite a lot of the original unit test framework code, so I doubt that roku would've merged it all back any time soon
2. It's conceptually entirely different: e.g. using annotations instead of naming conventions and boiler-plate code, completely different test reporting output, assertions and test cases maintain their own state, runs in a scenegraph scene, to name but a few
3. It has many more features than the original framework, not limited to : node specific assertions, exact assertion line failure reporting, better error messaging, easier setup, groupings, only and ignore for tests, mocks and stubs, etc, etc
4. Being completely frank, I enjoy roku work and want to do more of it, so it's useful to me to own this project, rather than lose control and wait on other's to merge my changes. On that note, email me at george[AT]tantawowa.com, or pm me (georgejecook) on the roku slack group to discuss any roku development requirements
5. I poured a _lot_ of work into the project (> 100 hours and counting), and expect to continue to do so. If I own the project, then I can do what I want, when I want. That goes for you guys as well, so get in touch with feature requests and PR's :)

### Is Rooibos itself unit tested?

At this point, it's WIP. I keep adding tests as bugs come up, and will continue to improve the test coverage. 

### Why 4.0.0?

Rooibos now uses the excellent bsc compiler plugin mechanism to seamlessly integrate with the compiler and the vscode IDE extension. This is a breaking change - projects will require updates to work.