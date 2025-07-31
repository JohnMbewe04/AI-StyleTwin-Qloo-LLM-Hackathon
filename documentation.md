# 👗 AI StyleTwin

AI StyleTwin is an AI-powered web app that helps users discover their fashion aesthetic based on the movies and music they love. Built during the **Qloo LLM Hackathon 2025**, it uses AI-driven cultural insights to match your taste with curated style recommendations and aesthetic outfit ideas.

---

## 📌 Table of Contents

- [Inspiration](#inspiration)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Demo Video](#demo-video)
- [How to Run](#how-to-run)
- [Challenges](#challenges)
- [What's Next](#whats-next)
- [License](#license)

---

## 💡 Inspiration

This project was inspired by a fashion-savvy friend who often struggles with the classic dilemma: _"I have nothing to wear."_ I realized that our media preferences—what we watch or listen to—often reflect how we feel. That insight sparked the idea: what if fashion recommendations could be powered by your favorite movies or songs?

---

## ✨ Features

- 🎬 Input a movie, genre, or song to get matched with fashion styles
- 🧠 Uses **Qloo's Taste AI** for cultural insights (with fallbacks to **TMDB**, **Spotify**, and **Last.fm**)
- 🧵 Maps vibes to fashion archetypes like grunge, techwear, cottagecore, etc.
- 🖼️ Shows real-world outfits using **Unsplash**, **Pexels**, or **Pixabay**
- 👗 Interactive virtual fitting room with image carousel
- 🌐 Multi-tab Streamlit UI: Media ➡ Fashion ➡ Try-On

---

## 🧰 Tech Stack

| Category     | Tools Used |
|--------------|------------|
| Language     | Python     |
| Framework    | Streamlit  |
| APIs         | Qloo, TMDB, Spotify, Last.fm, Unsplash, Pexels, Pixabay |
| Image Hosting | IMGBB     |
| Frontend Styling | HTML/CSS embedded in Streamlit |
| Secrets Management | `st.secrets` |

---

## 🎥 Demo Video

Watch the full demo here:  
**👉 [YouTube Demo](https://www.youtube.com/watch?v=https://youtu.be/7uqX9SrTsu8)**

---

## 🚀 How to Run Locally

1. **Clone the repository**
```bash
git clone https://github.com/your-username/ai-styletwin.git
cd ai-styletwin
````

2. **Install dependencies**

```bash
pip install -r requirements.txt
```

3. **Add your `secrets.toml` file under `.streamlit/`**

```toml
[api]
qloo_key = "your_qloo_api_key"
tmdb_key = "your_tmdb_key"
unsplash_key = "your_unsplash_key"
lastfm_key = "your_lastfm_key"

[spotify]
client_id = "your_spotify_client_id"
client_secret = "your_spotify_client_secret"

[imgbb]
imgbb_api_key = "your_imgbb_key"
```

4. **Run the app**

```bash
streamlit run app.py
```

---

## 🧩 Challenges

* Qloo’s API required detailed URN handling and returned sparse data at times, which led to building robust fallbacks.
* Streamlit was easy to use but limited in layout flexibility, requiring creative workarounds for tab navigation and interactivity.
* Managing multiple APIs, rate limits, and user input variability required strong caching and logic flow.

---

## 🔮 What's Next

* Add user profiles with persistent taste memory
* Integrate real-time shopping APIs (ASOS, Amazon Fashion)
* Add AR-based try-ons and mobile-first interface
* Expand to global fashion aesthetics and inclusive archetypes

---

## 📄 License

This project is licensed under the MIT License.

---

## 🙌 Acknowledgments

Thanks to Qloo, Streamlit, and all open-source contributors who made this project possible.

