# Web Perf like it's 2017

Note:

---

# 🤓 Csaba Palfi

[@csabapalfi](https://twitter.com/csabapalfi)

doing web for ~10 years

ex-(Hotels.com • Yahoo! • FT.com • TES • trainline + YLD)

now: HomeAway.com

Note:

doing web for around 10 years now at lots of different sites

thanks to YLD for organizing the meetup

consultant at HomeAway helping out with landing pages

we care about performance

---

# 🙋 
How many people here are NOT web developers?

(or full-stack)

Note:

Any non-web developers? 

Sorry, will try to make it interesting.

Tell your friends

---

Today we're going to talk about...

## ~~🤹 tips and tricks~~

## 📏 measurements

Note:

You can't improve what you can't measure.

Gives you a mental model, too and helps optimizing.

---

...more specifically

## 😍 user-centric metrics <!-- .element: class="fragment" -->

## 👥 real user-monitoring <!-- .element: class="fragment" -->

Note:

Leveraging performance metrics that affect user experience.

Measuring the perception of real users in production.

---

# 🏁 What is 'fast'?

`DOMContentLoaded`? `load`? 

a single metric won't do <!-- .element: class="fragment" -->

user experience? <!-- .element: class="fragment" -->

---

# 👫 How users think?

---

<!-- .slide: data-background="img/happening_ha.png" data-background-size="contain" -->

---

<!-- .slide: data-background="img/meaningful_ha-small.png" data-background-size="contain" -->

---

<!-- .slide: data-background-video="video/usable_ha.mp4" data-background-size="contain" data-background-video-loop="true" -->

---

# 👫 How users think?

🔜 happening?

🤔 meaningful?

👆 usable?

🥃 smooth?

---

# 🛠️ Metrics from?

![](img/webpagetest.png)  <!-- .element: class="fragment" --> ![](img/speedcurve.png)  <!-- .element: class="fragment" --> ![](img/lighthouse.png)  <!-- .element: class="fragment" -->

![](img/browsers.png)  <!-- .element: class="fragment" -->

<!-- .slide: data-background-color="#232323" -->

---

# <span style="filter: invert(100%);">🔜</span> happening?

* first pixel on the screen?
* Start render - WebPageTest

<!-- .slide: data-background-color="#232323" -->

---

![](img/paint-timing.png)

https://w3c.github.io/paint-timing/

`first-paint` / `first-contentful-paint`

---

# 🤔 meaningful?

* Visually Complete - WebpageTest.org
* Time to First Meaningful Paint - LightHouse
* Speed Index - both

<!-- .slide: data-background-color="#232323" -->

Note:

https://ldnwebperf.org/events/speed-perception-and-lighthouse/

---

# Hero Element Timing

![](img/hero-element-timing.png)

<!-- .slide: data-background-color="#232323" -->

Note:

https://docs.google.com/document/d/1yRYfYR1DnHtgwC4HRR04ipVVhT1h5gkI6yPmKCgJkyQ/edit#

https://github.com/w3c/charter-webperf/issues/30

https://github.com/tdresser/hero-element-polyfill

https://speedcurve.com/blog/user-timing-and-custom-metrics/
https://speedcurve.com/blog/web-performance-monitoring-hero-times/

---

# 👆 usable?

* User Timing `mark`s

<!-- .slide: data-background-color="#232323" -->

--- 

# 👆 usable?

* Time to Interactive

<!-- .slide: data-background-color="#232323" -->

Note:

https://github.com/GoogleChromeLabs/tti-polyfill

---


![](img/long-task.png)

https://w3c.github.io/longtasks/


---

# 🥃 smooth?

* Estimated Input Latency (LightHouse)

* DIY in `eventListener`
```js
const lag =
    performance.now() - 
    event.timeStamp;
```

<!-- .slide: data-background-color="#232323" -->

---

# 👫 User-centric metrics

🔜 happening? Start render, FP, FCP

🤔 meaningful? Visually complete, FMP, hero elements

👆 usable? custom marks, TTI

🥃 smooth? input latency, long-tasks

---

# How do you measure?

* synthetic
* real user monitoring

---

# Ok, why RUM?

* not all users have the same experience

---

# RUM challenges

* measurement browser support
* implementation lives in production code
* telemetry loss bias

---

# Load abandonment

* track `visibilitychange`
* small amount of blocking JS in `<head>`

---

# Synthetic

* all the metrics
* do it before production! (too)

---

# Summary

* measure user centric metrics
* use synthethic measurements in your pipeline
* validate/track real users in production

---

# Thanks, questions?