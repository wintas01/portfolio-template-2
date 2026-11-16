# Portfolio Template 2 — ECHO 🎬

A cinematic, scroll-driven portfolio that feels like watching a film. It's **one single file** (`index.html`), so you don't need to install anything, and you don't need to know React or any framework.

**What happens as you scroll**
1. **Intro:** a glowing logo with a wobbly outline that draws itself, then blurs into the site
2. **Hero:** a giant "EXPLORE MY PORTFOLIO" headline with your portrait in front
3. **About:** a black-and-white swirly starry sky. The "ABOUT ME" card splits open and grows into a full-screen light-beam scene, and the text scrambles into place
4. **Experience:** glowing titles slide sideways over giant faded text, one panel per job
5. **Featured projects:** your landing pages sit on a curved 3D ribbon that turns as you scroll
6. **Services and Contact**

---

## 🚀 How to use this template

### Step 1 — Get your own copy
Pick **one** of these:
- **Easiest:** click the green **Code** button → **Download ZIP**, then unzip it on your computer.
- **On GitHub:** click **Fork** (top right) to copy the repo into your own account.

### Step 2 — Open it
Double-click `index.html` and it opens in your browser. That's your website.

To edit it, open `index.html` in a code editor. [VS Code](https://code.visualstudio.com/) is free; Notepad works too.

> 💡 **Tip:** to find the text you want to change, press **Ctrl + F** (Windows) or **Cmd + F** (Mac) in your editor and search for it. Change it, save the file, then refresh the browser to see the result.

---

## ✏️ Step 3 — Put in your details

Search for each item in the left column and replace it with your own.

| Search for | What it is | Change it to |
|---|---|---|
| `ECHO` | Your brand name: the loading screen logo, top-left logo and browser tab title | Your name or brand (short names look best) |
| `Your Name` | Footer | Your full name |
| `Your City` | Hero and About sections | Your city |
| `Creative developer` | Small text on the left of the hero | Your job title |
| `Crafting interactive websites` | Small text on the right of the hero | What you're currently doing |
| `EXPLORE MY` / `PORTFOLIO` | Giant hero headline | Keep it, or write your own (two short lines) |
| `DISCOVER &amp; CRAFT` | About heading (`&amp;` means "&") | Your own heading |
| `I'm a creative developer` | About paragraph | A few sentences about you |
| `Self-taught` / `Builder` | Small tags above the About heading | Words that describe you |
| `Where<br>I've been` | Experience intro title (`<br>` = new line) | Keep it or change it |
| `Creative<br>Technologist` | 1st job title | Your job title |
| `2022 <span></span> 2023` | Dates for that job | Your dates |
| `Self-directed learning` | Company or type of role | Your company |
| `An intensive self-education` | Description of that job | What you did there |
| `Focus` / `Stack` | Small facts under each job | Your own facts |
| `Full Stack<br>Developer` and `Founder &amp;<br>Lead Designer` | 2nd and 3rd jobs | Same as above. Also update `data-label="..."` on each `<div class="panel">`, which is the small label at the top left |
| `Landing Pages` (in Services) | The 4 services you offer | Your services |
| `hello@yourname.com` | Email in the Contact section (appears 2 times on one line) | Your email |
| `aria-label="Instagram"` (and X, GitHub) | Social icons at the top right | Replace `href="#"` with your profile links |

> **Adding or removing jobs:** copy a whole `<div class="panel" ...> ... </div>` block in the Experience section and paste it below the others. The slider adjusts automatically. Remember to update the numbers like `01 / 03`.

---

## 🖼️ Step 4 — Add your own photo

1. Create a folder called **`images`** next to `index.html`.
2. Add a photo of yourself named **`me.png`**. A photo with the **background removed** looks best; you can do this free at [remove.bg](https://www.remove.bg).
3. In `index.html`, search for `PORTRAIT`. Just below that note is a block that starts with `<svg class="portrait"` and ends with `</svg>`. Replace that **whole block** with:
   ```html
   <img class="portrait" id="portrait" src="images/me.png" alt="Your Name">
   ```

---

## 🧩 Step 5 — Add your projects to the 3D ribbon

Search for `const pages=[`. Each line inside it is one project on the ribbon. To use a real screenshot, write an entry like this:

```js
{name:'My Shop', type:'E-commerce site', img:'images/my-shop.jpg', link:'https://myshop.com'},
```

- `name`: the project name shown under the ribbon
- `type`: a short description
- `img`: your screenshot in the `images` folder. Landscape images (about 16:10) look best.
- `link` (optional): where someone goes when they click the project

You can delete the example projects you don't need. The ribbon looks best with **6 to 10 projects**.

---

## 🎨 Change the colours (optional)

Near the top of `index.html`, look for `:root{`:

```css
--paper:#ebeae6;   /* light background (hero and projects) */
--ink:#0b0b0b;     /* dark text */
--night:#050505;   /* dark background (about, experience, services) */
```

---

## 🌍 Step 6 — Put it online (free)

**Option A: GitHub Pages**
1. Upload your edited files, including the `images` folder, to your own GitHub repo, or edit them directly in your fork.
2. In the repo, go to **Settings → Pages**.
3. Under **Source**, choose **Deploy from a branch**, pick **main** and **/ (root)**, then click **Save**.
4. Wait about 1 minute. Your site will be live at `https://YOUR-USERNAME.github.io/REPO-NAME/`.

**Option B: Netlify (drag and drop)**
Go to [app.netlify.com/drop](https://app.netlify.com/drop) and drag your project folder onto the page. It goes live instantly.

---

## ❓ Common questions

- **I broke something!** Undo your last change (Ctrl + Z) or download a fresh copy. Usually a `<`, `'` or `"` was deleted by mistake.
- **My photo doesn't show.** Check that the file name matches exactly. `Me.PNG` and `me.png` are different on GitHub Pages.
- **The starry sky looks different each time.** That's on purpose. It's drawn fresh by code on every visit.
- **Does it work on phones?** Yes. The scroll scenes adapt to smaller screens.

---

Free to use for your personal portfolio. If it helps you, a ⭐ on the repo is appreciated!
