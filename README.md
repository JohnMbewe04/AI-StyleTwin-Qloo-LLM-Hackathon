# AI-StyleTwin-Qloo-LLM-Hackathon

**AI StyleTwin** is a fashion recommendation web app that helps users discover their personal aesthetic by analyzing the movies and music they love.

Built during the Qloo LLM Hackathon, it connects media preferences with fashion archetypes using a combination of AI, cultural intelligence, and fallback logic—turning *“I have nothing to wear”* into *“This feels so me.”*

---

## 🎯 Inspiration

I was inspired by a close friend who's deeply into fashion, but often struggled with the all-too-familiar feeling: *"I have nothing to wear."* I realized the issue wasn't about having more clothes—it was about choosing what *felt right*.
That’s when the idea struck: our favorite movies and songs reflect our moods, identity, and vibe. So what if I could use those preferences to recommend outfits that align with them?

**AI StyleTwin** was born from that thought.

---

## 💡 What It Does

* 🎬 Accepts user input like **movie titles**, **genres**, or **songs**
* 🧠 Uses **Qloo’s Taste AI™** to predict style archetypes from cultural preferences
* 🔁 Falls back to **TMDB**, **Spotify**, and **Last.fm** if Qloo returns nothing
* 👗 Generates fashion outfit ideas using **Unsplash**, **Pexels**, or **Pixabay**
* 🌀 Displays styles in a dynamic **fitting room carousel**
* 📱 Enables media-inspired fashion discovery in an interactive, multi-tab layout

---

## 🛠 Built With

| Category           | Tools / Services                                        |
| ------------------ | ------------------------------------------------------- |
| **Framework**      | [Streamlit](https://streamlit.io/)                      |
| **APIs**           | Qloo, TMDB, Spotify, Last.fm, Unsplash, Pexels, Pixabay |
| **Image Hosting**  | IMGBB                                                   |
| **Languages**      | Python, HTML/CSS (embedded in Streamlit)                |
| **Auth & Secrets** | `st.secrets`                                            |

---

## 🚧 Challenges

* ❗ **Qloo API**: Difficult to implement due to undocumented URNs, inconsistent results, and strict authentication.
* 🧩 **Streamlit Limitations**: Layout control, tabbed navigation, and carousel integration required multiple creative workarounds.
* 🔁 **Fallback Logic**: I had to build genre-to-style mappings manually when data wasn’t available through APIs.

---

## 🏆 Highlights

* 🧠 Smart mapping from media to fashion archetypes
* 📸 Interactive visual fitting room with outfit carousels
* 🔄 Resilient API chaining with graceful degradation
* 🌍 Accessible design with global-friendly tech stack

---

## 📚 What I Learned

* How to design a fallback-first architecture around uncertain APIs
* How to simulate a full product UI/UX using Streamlit
* How subjective traits like "aesthetic" can still be modeled with logic
* That fashion tech needs to feel intuitive, not just functional

---

## 🔮 What's Next

* 🎨 AI-powered mood boards and style clustering
* 🛍️ Outfit shopping integration (e.g. ASOS, Amazon Fashion)
* 👤 User profiles with taste history and learning feedback loops
* 📱 AR try-ons and mobile-first design
* 🌐 Expansion to diverse fashion cultures and global vibes
