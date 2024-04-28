---
theme: apple-basic
title: "[Learn your way] - CQS / CQRS"
author: Maxime Miramond
layout: image
image: https://miro.medium.com/v2/resize:fit:4800/format:webp/1*q5Hf5tFYBkH8jnkM8e59rw.png
favicon: https://cqrs.nu/assets/cqrs_logo-0b4b17c2.png
fonts:
  sans: 'Roboto'
  serif: 'Roboto Slab'
  mono: 'Fira Code'
---

<div class="absolute bottom-5">
  <h1>[Learn your way] - CQS / CQRS</h1>
  <p>For beginners, by a beginner</p>
</div>

---
transition: fade-out
---

# CQS - Command Query Separation

<br><br>

<div style="width: 95%" class="text-2xl">

- ✍️ Commands — Change the state of a system but do not return a value

<br>

- 🤌 Queries — Return a value and don't change the state of the system (side-effect free)

</div>

---
transition: fade-out
---

# Why does this matter?

<br>

<div style="width: 95%" class="text-2xl">

- 🔒 By enforcing this separation, the code becomes simpler to understand

<br>

- 🔄 Is this changing something, or just fetching something?

<br>

- 🤔 When a method does both (changes the state of the application and retrieves data), it becomes a lot harder to understand it's true purpose

<br>

- 🧩 This can lead to really hard to reason about application state

</div>

---
transition: fade-out
---

# CQRS - Command Query Responsibility Segregation

<br><br>

<div style="width: 95%" class="text-2xl">

- 🖖 **CQRS** is about separate models for writes and reads

<br>

- 🗃️ We could have two different databases for reading and writing

<br>

- 🖇️ There is a fairly common confusion between the two in everyday language

</div>

---
transition: fade-out
---

# 3 Most Common Misconceptions about CQRS

<br>

<div style="width: 95%" class="text-xl">

- 🗄️ Multiple Databases
  - 🤷 Not necessarily, but yeah it's could be a good idea

- 📚 Event Sourcing
  - 🤝 Not necessarily, but it's a good fit

- 📨 Asynchronous Messaging
  - 📬 Do not need to be using a message bus to apply CQRS
  - ⏭️ Commands do not need to be asynchronous
  - 🔄 Everything can be done in a synchronous request/response manner

</div>

---
transition: fade-out
---

<img src="https://github.com/miramo/cqrs-training/blob/main/assets/images/greg-cqrs.png?raw=true" style="display:block;float:none;margin-left:auto;margin-right:auto;height:90%">

---
transition: fade-out
---

<br><br>

<img src="https://github.com/miramo/cqrs-training/blob/main/assets/images/cqrs-diag.png?raw=true" style="display:block;float:none;margin-left:auto;margin-right:auto;height:90%">

---
transition: fade-out
---

<div class="mt-10 flex justify-center items-center">
    <h1>Example / Questions?</h1>
</div>

<br>

<img src="https://i.giphy.com/media/3oKIPnAiaMCws8nOsE/giphy.webp" style="display:block;float:none;margin-left:auto;margin-right:auto;width:35%">
