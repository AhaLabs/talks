---
headingDivider: 1
style: |
  section {
    justify-content: flex-start;
    font-size: 2.5em;
  }
  section.joy a,
  section.joy h1 {
    color: rgb(93, 74, 93);
  }
  section.joy a {
    text-decoration: underline;
  }
---

# How Stellar's dApp Tooling Optimizes for Joy

A fast-paced "live coding" session.

<!-- Original submitted talk description: Crack open your laptop and follow along with this fast-paced live coding session. We'll use Stellar CLI to initialize a new dapp, take a look at the contracts, and quickly move onto building out our frontend app. We'll switch back and forth between tweaking the contracts and the frontend, helping you solidify your mental model of how it all fits together. We'll also look at how to build against a contract you didn't author, integrating it into your frontend toolset as easily as your own contracts. -->

---

![bg](joy/pattern-letters.webp)

# : j o y :

# 😂 

<!-- this always seemed TOO happy to mean "joy" to me! -->

---

![bg contain](joy/jesus.gif)

<!-- as an evangelical kid, I was taught that joy came from putting jesus first! and that it wasn't an extreme happiness, but a more foundational state of mind / orientation toward the world / aspect of character -->

---

![bg](joy/inside-out-joy.webp)

<!-- if you search for images of joy, you get a LOT of Inside Out -->

---

![bg](joy/jumping.jpg)

<!-- and also a lot of lens flare -->

---

![bg](joy/mindful-breath.jpeg)

<!-- like, a lot -->

---

![bg](joy/mountaintop.jpeg)

<!-- so much -->

---

![bg](joy/swing.webp)

<!-- on and on -->

---

![bg](joy/chatgpt.webp)


<!-- ChatGPT will give you lens flares, too. Why lens flares, I asked. "Lens flares are often associated with joy because they evoke the brightness and energy of sunlight, which is commonly linked to positive emotions like warmth, happiness, and freedom. Visually, lens flares can create a sense of liveliness and motion in an image, enhancing the dynamic quality of the scene. When used in moments that feature bright sunlight, the effect can highlight the carefree, radiant feeling often associated with joyful experiences, like playing outdoors, celebrations, or simply basking in a beautiful day." -->

---

![bg](joy/raincoat-smile.png)

# joy

_noun_

- Intense and especially ecstatic or exultant happiness, or an instance of such feeling.

# joy

_noun_

- Intense and especially ecstatic or exultant happiness, or an instance of such feeling.

&nbsp;

&nbsp;

The American Heritage® Dictionary of the English Language, 5th Edition

# joy

_according to Merriam-Webster_

* the emotion evoked by well-being, success, or good fortune

# joy

_according to Merriam-Webster_

- the emotion evoked by well-being, success, or good fortune or by the prospect of possessing what one desires

# joy

_according to Merriam-Webster_

- the emotion evoked by well-being, success, or good fortune or by the prospect of possessing what one desires, _delight_
* a source or cause of delight


# stellar

<!--
backgroundImage: "url(./joy/bg.webp)"
class: joy
-->

<!-- joy is the default! i'll mark parts of the developer journey that lack joy -->


# stellar-cli

* install [rust](https://developers.stellar.org/docs/build/smart-contracts/getting-started/setup#install-rust), then
* `cargo install cargo-binstall`
* `cargo binstall stellar-cli`

# short help

the default

* `stellar`
* `stellar -h`

# long help

is long

* `stellar --help`
* `stellar --help | less`

# network

* `stellar network container start local`
* `stellar network container logs local`
* `stellar network ls -l`

# network

- `stellar network container start local`
- `stellar network container logs local`
- `stellar network ls -l`

```
Default
Name: local
Network {
    rpc_url: "http://localhost:8000/rpc",
    network_passphrase: "Standalone Network ; February 2017",
}
```

# getHealth

<!--
_backgroundImage: none
_class: ohno
-->


* `curl -s -X POST "http://localhost:8000/soroban/rpc" -H "Content-Type: application/json" -d '{ "jsonrpc": "2.0", "id": 8675309, "method": "getHealth" }' | sed 's/.*"status":"\([^"]*\)".*/\1/'`
* if `healthy`, it's ready!

<!-- no joy here. save it! -->

# keys

* `stellar keys generate alice`
* `stellar keys fund alice`

# send tokens

* `stellar keys generate bob`
* `stellar`

# send tokens

- `stellar keys generate bob`
- `stellar...`

# send tokens??

<!--
_backgroundImage: none
_class: ohno
-->

- `stellar keys generate bob`
- `stellar...`

# contract

* `stellar contract id asset`
* `stellar contract init`
* `stellar contract build`
* `stellar contract deploy`
* `stellar contract invoke`
* `stellar contract bindings`
