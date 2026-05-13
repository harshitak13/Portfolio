# ✦ Harshita Karnam — Personal Portfolio

A bold, vibrant personal portfolio website built with vanilla HTML, CSS, and JavaScript. No frameworks, no build tools — just clean code that deploys anywhere in seconds.

## 🌐 Live Site

> [harshitak13.github.io/portfolio](https://harshitak13.github.io/portfolio) ← update this link after deploying

---

## ✨ Features

- **Fully responsive** — looks great on mobile, tablet, and desktop
- **Animated UI** — floating gradient blobs, scroll-reveal animations, morphing shapes
- **Contact form** — powered by EmailJS, messages land directly in your inbox (no backend needed)
- **Zero dependencies** — single `index.html` file, nothing to install
- **Fast** — no frameworks, loads instantly

---

## 🚀 Deployment

### GitHub Pages (recommended)

```bash
git clone https://github.com/harshitak13/portfolio.git
cd portfolio
# add your index.html, then:
git add .
git commit -m "init: portfolio site"
git push origin main
```

Then go to **Settings → Pages → Source → main branch → Save**.
Your site will be live at `https://harshitak13.github.io/portfolio`.

### Netlify (one click)

Drag and drop `index.html` at [netlify.com/drop](https://app.netlify.com/drop) — live in 30 seconds.

---

## ⚙️ EmailJS Setup

The contact form uses [EmailJS](https://www.emailjs.com) to send messages straight to your inbox — free, no backend required.

1. Create a free account at [emailjs.com](https://www.emailjs.com)
2. Add an **Email Service** (Gmail recommended) and note your **Service ID**
3. Create an **Email Template** using these variables:

```
From: {{from_name}} ({{reply_to}})
Subject: {{subject}}

{{message}}
```

4. Copy your **Template ID** and **Public Key** (under Account → General)
5. Open `index.html` and replace the three placeholders:

```js
emailjs.init("YOUR_EMAILJS_PUBLIC_KEY");
emailjs.sendForm('YOUR_SERVICE_ID', 'YOUR_TEMPLATE_ID', this)
```

---

## 🗂 Project Structure

```
portfolio/
└── index.html      # Everything lives here — HTML, CSS, and JS in one file
```

---

## 🎨 Customisation

All colours are CSS variables at the top of the `<style>` block — easy to swap out:

```css
:root {
  --yellow:  #f5e642;
  --pink:    #ff4d8d;
  --cyan:    #00e5ff;
  --green:   #39ff84;
  --purple:  #b44dff;
}
```

---

## 📄 License

Open source under the [MIT License](LICENSE). Feel free to use this as a template for your own portfolio — a credit or star is always appreciated. ⭐

---

<p align="center">Built by <strong>Harshita Karnam</strong> · <a href="mailto:harshita.karnam909@gmail.com">harshita.karnam909@gmail.com</a></p>
