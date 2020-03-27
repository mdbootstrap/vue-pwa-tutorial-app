# [The app](https://mdb-vue-pwa.firebaseapp.com/)

# Material Design for Bootstrap Vue PWA tutorial
The repo contains an exemple agenda app in different stages and the tutorial content, describing the codes' ascention to a Progressive Web App. 
It goes step by step, requiring no sophisticated tooling beyond Vue and webpack nor a git skill.

## Reasoning
I acknowledge there are some great scaffolding methods, which allow you to have the PWA with a snap of the fingers (most notably the vue-cli's PWA extension), so one could never have to do the manual labour presented here in their professional life, ever. I know from my own experience, that such tools, although amazingly handy, do most of the things in a "under the hood" fashion, obscuring the important details of the job. The tutorial is aimed at people who want to enhance their understanding of what a PWA actually entails, what it requires and how to apply its principals to an existing Vue app. To that end, it was consciously made slow-paced and manual.

It has two features which I especially value: first, a custom webpack config, which is something rarely seen these days, replaced in favor of more abstract, framework-scaffolding tooling (be it `create-react-app` or `vue-cli` or whatever). Secondly, the project is made using the MDBVue library (which I spent over a year developing), offering beautiful material design components to developers, high customization potential to apps and now, with tree-shaking, easy on the browser.

## Structure
The tutorial ("the documentation") will be available on the MDB website soon, with the repo here reduced to just the app code and, I assume, forked and hosted on the offial MDB account. As of now, though, I am developing these two _faci_ alongside each other in one repo for convenience reasons, at least for now.

The tutorial starts where the MDB introductory course into Vue left off, and as such it assumes no new `git` ability of the _neophite_. Because of this, the consequtive steps are presented in separate folders within the `app/` directory, rather than on different branches. I am not a fan of this solution for many reasons (most notably because I consider `git` an essential tool for anyone interested in web-development and the FOSS culture, which should not be shun away from), but hey - at least it stays consistent with its precessor.
