# Web Perf like it's 2017

---

# 🤓 Csaba Palfi

[@csabapalfi](https://twitter.com/csabapalfi)

doing web for ~10 years

ex-(Hotels.com • Yahoo! • FT.com • TES • trainline + YLD)

now: HomeAway.com

---

# 🙋 
How many people here are NOT web developers?

(or full-stack)

---

Today we're going to talk about...

## ~~🤹 tips and tricks~~

## 😍 user-centric metrics

## ⚗️ lab vs real users

---

# ⚡ How fast are you?

Time to first byte <!-- .element: class="fragment" -->

`DOMContentLoaded` <!-- .element: class="fragment" -->

`load` <!-- .element: class="fragment" -->

---

# 👫 What users think?

🔜 happening? <!-- .element: class="fragment" -->

🤔 meaningful?  <!-- .element: class="fragment" -->

👆 usable? <!-- .element: class="fragment" -->

🥃 smooth? <!-- .element: class="fragment" -->

---

# 🛠️ How to measure?

* LightHouse  <!-- .element: class="fragment" -->
* WebpageTest.org  <!-- .element: class="fragment" -->
* the browser!  <!-- .element: class="fragment" -->

---

# 🔜 happening?

* Start render
* `first-paint`
* `first-contentful-paint`

---

# 🤔 meaningful?

* Visually Complete
* Time to First Meaningful Paint
* Hero Element Timing 

Note:

elementtiming
https://speedcurve.com/blog/user-timing-and-custom-metrics/
https://speedcurve.com/blog/web-performance-monitoring-hero-times/

---

# 👆 usable?

* User Timing `mark` (e.g. in `componentDidMount`)
* Time to Interactive

---

# 🥃 smooth?

* absence of long tasks, input latency

---

filmstrip

---

# How do you test?

* locally
* locally/lab with throttling CPU/network
* real user monitoring

---

# How to measure

# emoji 
Is Lighthouse/Webpagetest.org accurate?

---

#3G

---

Synthetic tests are most useful to see differences before/after deployment.

What do real users experience: RUM

---


---

# Load abandonment

survivorship bias
telemetry loss bias

---

Browser support?

---

# Summary

* measure user centric metrics
* use synthethic measurements in your pipeline
* validate/track real users in production

---

# THE CUT

---

# state of the web

https://whatdoesmysitecost.com/#gniCost
https://www.akamai.com/us/en/solutions/intelligent-platform/visualizing-akamai/internet-observatory/

---

# budgets

https://infrequently.org/2017/10/can-you-afford-it-real-world-web-performance-budgets/


http://mi.eng.cam.ac.uk/~cipolla/archive/Presentations/MakingPresentations.pdf

https://developers.google.com/web/updates/2017/06/user-centric-performance-metrics
