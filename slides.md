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

---

# Modern web performance is a mess

Google showing the way
their business depends on it
money spent on crawlers, haha
build a mental model

---

Today we're going to talk about...

## ~~🤹 tips and tricks~~

## 😍 user-centric metrics

## ⚗️ lab vs real-user monitoring

---

# ⚡ How fast is your site?

`DOMContentLoaded` <!-- .element: class="fragment" -->

`load` <!-- .element: class="fragment" -->

---

# 👫 What users think?

🔜 happening? <!-- .element: class="fragment" -->

🤔 meaningful?  <!-- .element: class="fragment" -->

👆 usable? <!-- .element: class="fragment" -->

🥃 smooth? <!-- .element: class="fragment" -->

https://developers.google.com/web/updates/2017/06/user-centric-performance-metrics

---

# 🔜 happening?

* FP (Start render), FCP

---

# 🤔 meaningful?

* FMP, Hero element timing, (Speed Index, Visually Complete)
https://speedcurve.com/blog/user-timing-and-custom-metrics/
https://speedcurve.com/blog/web-performance-monitoring-hero-times/

---

# 👆 usable?

* Custom event handlers added, First interactive, Consistently interative

---

# 🥃 smooth?

* absence of long tasks, input latency

---

filmstrip

---

# emoji 
Is Lighthouse/Webpagetest.org accurate?

---

#3G

---

Synthetic tests are most useful to see differences before/after deployment.

What do real users experience: RUM

---

`PerformanceObserver` - tti, 

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
