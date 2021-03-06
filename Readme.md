![oh no](https://user-images.githubusercontent.com/914228/37348426-431dcaa6-2691-11e8-9e41-91fb5a5f0e5c.png)

# EmberConf 2018

A collection of links (and notes) that summarize the events of EmberConf 2018. Please submit a PR if you'd like!

Inspired by [**@poteto**](https://github.com/poteto)'s past EmberConf repos. See [2017](https://github.com/poteto/emberconf-2017), [2016](https://github.com/poteto/emberconf-2016), and [2015](https://github.com/poteto/emberconf-2015) for previous years!

## Livestream

> <img alt="" src="https://user-images.githubusercontent.com/914228/34072730-9d2d0bcc-e25a-11e7-9ab5-405ddce05303.gif" width="25"> <img alt="" src="https://user-images.githubusercontent.com/914228/34072749-07a8ab50-e25b-11e7-80ba-d0f6250aad11.png" width="20.5">

- [Official live stream](https://www.youtube.com/watch?v=qfnkDyHVJzs&feature=youtu.be)
- [Live captions](http://streamtext.net/player?event=Tilde)

## Job board

See photos [here](https://github.com/nucleartide/emberconf-2018/tree/master/job-board). Pictures were taken around 1 PM PST on Wednesday March 14.

## Day 1

### Talks

#### Keynote by [Tom Dale](https://twitter.com/tomdale) and [Yehuda Katz](https://twitter.com/wycats)

_Overall, lots of API improvements, as well as exciting advances in Glimmer.js._

- New filesystem layout
- Optional jQuery
- Codemods
  - `async`/`await` in tests
  - JS module api
  - Computed properties, use es5 getters
  - ES6 classes
    - TypeScript
  - Decorators
- Editor integration
  - [VSCode](https://code.visualstudio.com/docs/languages/typescript)
- Fragment components, empty tagName
- `@tracked` properties, autotracking dependencies
- `@args` syntax in templates
- Experimental
  - Angle bracket syntax
  - Single word component names
  - Named blocks RFC
- [LinkedIn feed in Preact and Glimmer](https://engineering.linkedin.com/blog/2018/03/how-we-built-the-same-app-twice-with-preact-and-glimmerjs)
- https://schedule.emberconf.com - uses rehydration
- https://schedule-wasm.emberconf.com - uses WASM
  - [Glimmer written in Rust](https://github.com/glimmerjs/glimmer-vm/pull/752)

#### Brief interlude from sponsor [Percy.io](https://percy.io) by [Mike Fotinakis](https://twitter.com/mikefotinakis?lang=en)

- [percy-web](https://github.com/percy/percy-web), open source front-end
- [Example of PR integration](https://github.com/percy/percy-web/pull/459)

#### Ambitious for All: Accessibility in Ember by [Melanie Sumner](https://twitter.com/melaniersumner?lang=en)

> Be magnanimous.

- [Video](https://youtu.be/qfnkDyHVJzs?t=8286)
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- WAI-ARIA
- WCAG 2.0
- [Color-blind glasses](https://www.google.com/search?q=color+blind+glasses)
- https://include.ai
  - Add alt text to images on the web
- [ember-a11y](https://github.com/ember-a11y)
- Problems
  - Route transitions
  - Modal focus
  - `aria-*` support
  - Clicks
  - Passwords
- Easy wins
  - Use HTML5 elements
  - Link for routing, button for everything else
  - Keyboard nav, arrow keys
  - [Color contrast](https://a11ywins.tumblr.com/post/167324368213/google-chromes-color-contrast-debugger)
  - Image alt text
    - `<img src="elmo.png" alt="" role="presentation" />`
- [`ember-component-attributes`](https://github.com/mmun/ember-component-attributes)
- [\#topic-a11y](https://embercommunity.slack.com/messages/C06MC4CG6/)

#### Everything they didn't tell you about the Ember Community by [Jessica Jordan](https://twitter.com/jjordan_dev)

_Jessica provides an exhaustive overview of the Ember.js ecosystem and Emberista subculture._

- [Video](https://youtu.be/qfnkDyHVJzs?t=10835)
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Subculture
  - Emberistas, subset/subculture of JavaScript community
- [Growth in `@angular/cli` download counts](https://npm-stat.com/charts.html?package=%40angular%2Fcli&from=2017-03-01&to=2018-03-13)
- Top addons on [Ember Observer](https://emberobserver.com/lists/top-addons)
- [`ember-rickroll`](https://github.com/nucleartide/ember-rickroll) :troll:
- [Ember Request For Comments (RFC) process](https://github.com/ember-cli/rfcs)
- Quest issues concept
  - Example: [Ember Data](https://github.com/emberjs/data/issues/5292)
- [Ember.js status board](https://www.emberjs.com/statusboard/)
- [Adoption of RFC process by React](https://reactjs.org/blog/2017/12/07/introducing-the-react-rfc-process.html)
- [Ember.js Slack Community](https://embercommunity.slack.com)
  - [`#give-wrjblue-a-beer`](https://embercommunity.slack.com/messages/C05599BQX/)
- [Rapidly growing `ember-cli-typescript` adoption](https://github.com/typed-ember/ember-cli-typescript)
- Email newsletters
  - [Ember Weekly](http://www.emberweekly.com/)
  - [Ember.js Times](https://the-emberjs-times.ongoodbits.com/)
- Offline
  - EmberConf
  - EmberFest
  - EmberCamp
  - Meetups
- [Ember Women Helping Women program](http://emberwomen.com/)
- (not part of talk, related essay) [Melancholy of Subculture Society](https://www.gwern.net/The%20Melancholy%20of%20Subculture%20Society)

#### The Next Generation of Testing by [Tobias Bieniek](https://twitter.com/tobiasbieniek?lang=en)

_Tobias introduces new, elegant testing APIs in Ember._

- [Video](https://youtu.be/qfnkDyHVJzs?t=17882)
- [Slides](https://speakerdeck.com/turbo87/the-next-generation-of-testing-in-ember-dot-js)
- `.andThen()` vs `async`/`await`
- [`ember-native-dom-helpers`](https://github.com/cibernox/ember-native-dom-helpers)
- [`@ember/test-helpers`](https://github.com/emberjs/ember-test-helpers)
- [Grand Testing Unification RFC](https://github.com/rwjblue/rfcs/blob/42/text/0000-grand-testing-unification.md)
- Codemods
  - [`ember-native-dom-helpers-codemod`](https://github.com/simonihmig/ember-native-dom-helpers-codemod)
  - [`ember-qunit-codemod`](https://github.com/rwjblue/ember-qunit-codemod)
  - [`ember-test-helpers-codemod`](https://github.com/simonihmig/ember-test-helpers-codemod)
- Test loading states: `await waitFor('.loading-spinner');`
- [`ember-test-selectors`](https://github.com/simplabs/ember-test-selectors)
- DOM assertion library: [`qunit-dom`](https://github.com/simplabs/qunit-dom)

#### Say More by [Jamie White](https://twitter.com/jgwhite)

Jamie examines test abstractions, and how one might hide details and edge cases behind a less powerful test language.

- [Video](https://youtu.be/qfnkDyHVJzs?t=20356)
- Slides - [https://speakerdeck.com/turbo87/the-next-generation-of-testing-in-ember-dot-js](https://speakerdeck.com/turbo87/the-next-generation-of-testing-in-ember-dot-js)
- Access via accessibility
- [Rule of Least Power](https://www.w3.org/2001/tag/doc/leastPower.html)
- [Babel plugin](https://babeljs.io/docs/plugins/) for generating `keyboardClick` test
- [`say-more`](https://github.com/jgwhite/say-more) app demonstrating concepts from talk

#### Who Moved My Cheese? Ember's New Filesystem Layout by [Matthew Beale](https://twitter.com/mixonic)

- [Video](https://youtu.be/qfnkDyHVJzs?t=22950)
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- [Ember.js Community Survey](https://emberjs.com/ember-community-survey-2018/)
- [Module Unification RFC](https://github.com/emberjs/rfcs/blob/master/text/0143-module-unification.md)
- Codemods
  - [ember-cli/ember-modules-codemod](https://github.com/ember-cli/ember-modules-codemod)
- [ember-optional-features](https://github.com/emberjs/ember-optional-features)
- Concepts
  - Colocation
  - Local lookup / isolation
  - Addon namespaces
    - `{{gadget-tools::list}}`
  - Compatibility between Module Unification layout and classic layout
- [schedule.emberconf.com](https://schedule.emberconf.com) module unification app
- [Quest issue, module unification: final cut](https://github.com/emberjs/ember.js/issues/16373)

#### Mastering the Art of Forms by [Danielle Adams](https://twitter.com/adamzdanielle)

_Danielle dives into component and data design for use in form UI and UX._

- [Video](https://youtu.be/qfnkDyHVJzs?t=26963)
- Slides - https://slides.com/danielleadams/art-of-forms-ec18
- Design questions
  - Field type
  - Required
  - Dependency between inputs
- Data-loading component using `willRender`
  - Retries with [`ember-concurrency`](https://github.com/machty/ember-concurrency)
- [`ember-cp-validations`](https://github.com/offirgolan/ember-cp-validations)
- Concerns
  - Built-in validation in HTML5 inputs
  - Tab navigation order that makes sense
- [Blue Apron](https://www.blueapron.com/) - form examples on the site

#### How To Build A Bonfire: On Training and Hiring New Devs by [Taylor Jones](https://twitter.com/hiimtaylorjones)

- [Video](https://youtu.be/qfnkDyHVJzs?t=29267)
- [Slides](https://www.slideshare.net/TaylorJones89/how-to-build-a-bonfire-on-hiring-and-training-ember-developers)
- [Mythical Man Month](https://en.wikipedia.org/wiki/The_Mythical_Man-Month)
  - Can't throw people at a problem... or can you :shipit:
- Help your team become _skilled_ at Ember
- "...context of a developer's past affects how they understand the future..."
  - Example: React vs. Angular background
- Have a style guide
  - Not just syntax, but how to do things

#### Living Animation by [Edward Faulkner](https://twitter.com/eaf4)

_mind blown_

- [Video](https://youtu.be/qfnkDyHVJzs?t=31861)
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Animation approaches
  - Tweening
  - Procedural animation: rules and physics models in games
- [liquid-fire](https://github.com/ember-animation/liquid-fire)
  - Separation between app logic and animation
  - Establish rules (like in games) and let motions emerge
- [`ember-animated`](https://github.com/ember-animation/ember-animated), "Glimmer"-ization of `liquid-fire`
- [ef4/living-animation](https://github.com/ef4/living-animation)

## Day 2

### Talks

#### The Future of Data in Ember by [Dan Gebhardt]()

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Links and notes:
  - None yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!

#### Smartphone Symphony by [Gavin Joyce](https://twitter.com/gavinjoyce)

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- [ember-present](https://github.com/GavinJoyce/ember-present)

#### Reuse, Recycle: One Team's Journey From Projects to Products by [Sarah Bostwick]()

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Links and notes:
  - None yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!

#### Deep Dive on Ember Events by [Marie Chatfield]()

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Links and notes:
  - None yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!

#### Building a Memex in Ember by [Andrew Louis]()

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Links and notes:
  - None yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!

#### Prying Open the Black Box by [Godfrey Chan]()

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Links and notes:
  - None yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!

#### Minitalk: Contributor Rally by [Sean Massa]()

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Links and notes:
  - None yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!

#### Minitalk: Toyota's Shared Component Library by [Tony Ward]()

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Links and notes:
  - None yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!

#### Minitalk: Lightning Thoughts on Lightning Deploy by [Christina Kung]()

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Links and notes:
  - None yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!

#### Minitalk: Let Me Ember This for You by [Serena Fritsch]()

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Links and notes:
  - None yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!

#### Creating Fluid App-Like Experiences With Ember by [Nick Schot]()

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Links and notes:
  - None yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!

#### Closing Keynote by [Saron Yitbarek]() and [Vaidehi Joshi]()

_No summary yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!_

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Links and notes:
  - None yet. Open a [PR](https://github.com/nucleartide/emberconf-2018/pulls)!
