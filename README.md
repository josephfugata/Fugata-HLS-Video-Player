# 🎬 HLS Video Player

A lightweight, self-contained **HLS video player** built with **conversion in mind**.
Created out of frustration with existing players that were either **too expensive**, **bloated**, or **not user-friendly enough** to keep viewers engaged.

Unlike other players, this one is:

* 💸 **Free** – no hidden fees, no premium lock-ins.
* 🎯 **Conversion-focused** – designed to **reduce drop-offs** and keep viewers watching.
* 🌐 **Easily deployable** – one HTML file, hostable on **Cloudflare Pages** or any static server.

---

## 💡 Why This Player Was Created

In marketing and customer engagement, **video drop-offs are highest in the first 10 seconds**.
According to [Wistia](https://wistia.com/learn/marketing/optimizing-video-for-engagement) and [HubSpot research](https://blog.hubspot.com/marketing/video-marketing-statistics), the top reasons viewers leave early are:

* **Confusing or slow start** – people don’t like waiting for playback.
* **Muted autoplay** without clear instructions.
* **Clunky controls** that make watching frustrating.
* **No personalization** (viewers have to restart every time they come back).

👉 This project was created to **solve those exact problems**.

### 🔑 How This Implementation Helps Conversion

* **Unmute overlay** → Removes the confusion of muted autoplay. Viewer sees *exactly* how to engage.
* **Resume playback** → Returning viewers don’t start over, they continue where they left off. This increases *completion rates*.
* **Big clear play button** → No clutter, just an immediate “play” action that works across devices.
* **Fast load (single file)** → No slow frameworks, so playback starts in seconds — critical for keeping attention.

In short, this player isn’t just for playing videos.
It’s for **maximizing the chance that someone actually finishes watching** — which is what drives conversions.

---

## 🚀 Features

* ✅ **HLS.js support** (non-Safari browsers)
* ✅ **Native HLS playback** (Safari support)
* ✅ **Overlay controls** (Play, Resume, Restart, Unmute)
* ✅ **Playback resume** (saves last watched timestamp in `localStorage`)
* ✅ **Autoplay handling** (with unmute prompt on first visit)
* ✅ **Single-file deployment** (just HTML + JS + CSS)

---

## 🌐 Hosting on Cloudflare Pages

You can deploy this project in just a few steps:

### 1. Fork or Clone this Repository

```bash
git clone https://github.com/your-username/hls-video-player.git
cd hls-video-player
```

### 2. Push to GitHub

Make sure your project is pushed to a GitHub repository.

### 3. Connect to Cloudflare Pages

* Go to **[Cloudflare Pages](https://pages.cloudflare.com/)**.
* Click **Create a Project** → **Connect to GitHub**.
* Select your repository.

### 4. Configure Build Settings

Since this is a static HTML project:

* **Framework preset:** None
* **Build command:** None
* **Output folder:** `/`

Click **Deploy** 🎉

---

## 🎥 Usage

Once deployed, pass the HLS video source via a query parameter:

```html
https://your-cloudflare-domain.pages.dev/?video=https://example.com/playlist.m3u8
```

### Example Embed (iframe)

```html
<iframe 
  src="https://your-cloudflare-domain.pages.dev/?video=https://example.com/playlist.m3u8" 
  width="800" 
  height="450" 
  frameborder="0" 
  allowfullscreen>
</iframe>
```

---

## 🛠 Local Development

You can preview the project locally by simply opening the `index.html` file in your browser.

Or run a simple static server:

```bash
# Using Python
python -m http.server 8080

# Using Node.js (http-server)
npx http-server .
```

Then visit:

```
http://localhost:8080/?video=https://example.com/playlist.m3u8
```

---

## 📂 Project Structure

```
hls-video-player/
├── index.html   # Main player
```

---

## ⚡ Tech Stack

* **[HLS.js](https://github.com/video-dev/hls.js/)** – For adaptive streaming support
* **Vanilla JS + HTML + CSS** – No frameworks, lightweight and fast

---

## 🙌 Tribute to the Struggle

This project was born from **countless hours of searching** for a simple, free, and conversion-focused player.
Most solutions were either:

* 🚫 Paid with high licensing costs
* 🚫 Over-engineered with features I didn’t need
* 🚫 Bad for conversions (users leaving early, muted autoplay confusion, no resume feature)

So I built my own.
If you’ve struggled with the same frustrations — this player is for you.

---

## 📜 License

I don't like to put one 😊. After all, technologies are for everyone.
 
