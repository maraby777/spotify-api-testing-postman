# 🎧 Spotify API Testing with Postman

A hands-on, exploratory + automated API testing project using [Spotify’s Web API](https://developer.spotify.com/documentation/web-api).  
Inspired by the Rapid Software Testing mindset — part journal, part workshop.

👩‍💻 Created by a QA engineer, for QA engineers. This is not just another tutorial, it's a field report.

---

## 🧭 Project Structure

This repo contains:

- 📄 **Article Series**: Exploratory journey through the Spotify API (see `articles/`)
- 🧪 **Postman Collections**: Reusable, versioned test cases for Spotify endpoints
- ⚙️ **Environment Files**: Postman environments with scoped variables
- 🤖 **Automation (ToDo)**: Plan for CI runs via GitHub Actions

---

## 🚀 Quick Start

> **Pre-reqs:** A Spotify Developer account and Postman installed.

1. Clone this repo or download the files
2. Go to [Spotify for Developers](https://developer.spotify.com/dashboard/)
3. Create your own app and get:
   - `client_id`
   - `client_secret`
   - set redirect URI to `http://localhost:8888/callback`
4. Import:
   - `Spotify_API_testing.postman_collection.json`
   - `Spotify_API_environment.postman_environment.json`
5. Follow the [authorization guide here](./articles/spotify-0-setup.md) to get your first token

---

## 📚 Article Series

- **Part 0 – Setup & Authorization Flow** → _Coming soon..._
- **Part 1 – Exploratory API Testing** → _Coming soon..._
- **Part 2 – Automating Collection** → _Coming soon..._
- **Part 3 – GitHub Actions Integration** → _Coming soon..._

---

## 🔬 What You'll Learn

- How to test APIs without writing code (but with logic!)
- How OAuth 2.0 really works when you're the one debugging it
- How to write resilient Postman scripts with scoped variables
- How to reason like a QA: find bugs, spot edge cases, write better tests

---

## 🐛 Known Bugs / Interesting Observations

> Based on real responses and edge cases from Spotify API.

- 502 on absurd `offset` instead of 400 → [Bug report](./articles/spotify-1-exploration.md#bug1)
- Inconsistent name length validation between API and UI
- Silent failures on missing scopes – API responds 403 but doc doesn’t mention it

---

## 💡 About the Author

Hi, I’m [Nat](https://www.linkedin.com/in/natashatereshchenko/) — a QA engineer with 10+ years in software testing.  
This repo is part of my open testing journal and career portfolio. Feel free to connect, reuse or fork!

---

## 🗂️ To Do

- [ ] Add test assertions across all requests
- [ ] Document dynamic variable generation
- [ ] Add Newman report automation
- [ ] Create GitHub Action for scheduled runs
