# [The app](https://mdb-vue-pwa.firebaseapp.com/)

# Material Design for Bootstrap Vue PWA tutorial
The repo contains an exemple agenda app in different stages and the tutorial content, describing the codes' ascention to a Progressive Web App. 
It goes step by step, requiring no sophisticated tooling beyond Vue and webpack nor a git skill.

## Reasoning
I acknowledge there are some great scaffolding methods, which allow you to have the PWA with a snap of the fingers (most notably the vue-cli's PWA extension), so one could never have to do the manual labour presented here in their professional life, ever. I know from my own experience, that such tools, although amazingly handy, do most of the things in a "under the hood" fashion, obscuring the important details of the job. The tutorial is aimed at people who want to enhance their understanding of what a PWA actually entails, what it requires and how to apply its principals to an existing Vue app. To that end, it was consciously made slow-paced and manual.

It has two features which I especially value: first, a custom webpack config, which is something rarely seen these days, replaced in favor of more abstract, framework-scaffolding tooling (be it `create-react-app` or `vue-cli` or whatever). Secondly, the project is made using the MDBVue library (which I spent over a year developing), offering beautiful material design components to developers, high customization potential to apps and now, with tree-shaking, easy on the browser.