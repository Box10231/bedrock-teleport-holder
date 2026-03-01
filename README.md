# Bedrock Teleport Holder Behavior Pack

This behavior pack adds one custom item: `bedrockmod:warp_relic`.

- Get it with: `/give @s bedrockmod:warp_relic`
- While holding it in your main hand or offhand, you are teleported to `8000 75 8000` every tick.

---

## Absolute beginner guide: put this on GitHub (step-by-step)

If you are new to GitHub, use **Method A (website only)**. It is the easiest.

## Method A (Easiest): Upload files with only the GitHub website

### 1) Create a new repo on GitHub
1. Go to https://github.com and sign in.
2. In the top-right, click the **+** button.
3. Click **New repository**.
4. In **Repository name**, type something like: `bedrock-teleport-holder`.
5. Choose **Public** (or **Private**, your choice).
6. Click **Create repository**.

### 2) Download this project as a ZIP
1. On this project page, click the green **Code** button.
2. Click **Download ZIP**.
3. Find the downloaded ZIP in your **Downloads** folder.
4. Right-click ZIP -> **Extract All...** (Windows) or double-click to extract.

### 3) Upload all files into your new GitHub repo
1. Open your new (empty) GitHub repo page.
2. Click **uploading an existing file**.
3. Open the extracted project folder on your computer.
4. Select these items and drag them into the browser upload box:
   - `manifest.json`
   - `README.md`
   - `items` folder
   - `functions` folder
5. Scroll down to **Commit changes**.
6. In message box, type: `Initial upload of behavior pack`.
7. Click **Commit changes**.

Done. Your files are now on GitHub.

---

## Method B: GitHub Desktop (still beginner-friendly)

### 1) Install and sign in
1. Install GitHub Desktop: https://desktop.github.com/
2. Open it and sign in to your GitHub account.

### 2) Add this folder
1. In GitHub Desktop, click **File -> Add Local Repository...**
2. Choose this project folder (the one with `manifest.json`).
3. If asked to create a repository, accept it.

### 3) Publish to GitHub
1. Click **Publish repository** in the top bar.
2. Choose a repo name.
3. Click **Publish Repository**.

Done. Your files are now on GitHub.

---

## Method C: Command line (copy/paste)

Use this if you already installed Git.

1. Create a new empty repo on GitHub first.
2. Open terminal in this project folder.
3. Copy/paste these commands (replace placeholders):

```bash
git init
git add .
git commit -m "Initial upload of behavior pack"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```

If it asks for login, complete GitHub sign-in in browser.

---

## Important: Is this automatic?

No. Changes are **not automatic** on GitHub.

You must either:
- Upload on the website,
- Click **Publish repository** / **Push origin** in GitHub Desktop, or
- Run `git push` in terminal.

---

## Install this behavior pack into Minecraft Bedrock

### Step 1: Find the correct pack folder
Use the folder that directly contains:
- `manifest.json`
- `items/`
- `functions/`

### Step 2: Copy that folder to the Minecraft behavior_packs location

#### Windows 10/11
1. Press **Windows key + R**.
2. Paste this path and press Enter:

```text
%LOCALAPPDATA%\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\LocalState\games\com.mojang\behavior_packs\
```

3. Copy your behavior-pack folder into this `behavior_packs` folder.

#### Android
Copy your behavior-pack folder to one of these:
- `/games/com.mojang/behavior_packs/`
- `/Android/data/com.mojang.minecraftpe/files/games/com.mojang/behavior_packs/`

#### iOS
Use Files app and copy the pack folder to:
- `On My iPhone > Minecraft > games > com.mojang > behavior_packs`

### Step 3: Activate in-game
1. Open Minecraft Bedrock.
2. Create a new world (or edit an existing one).
3. Open **Behavior Packs**.
4. Open **My Packs**.
5. Select **Bedrock Teleport Holder**.
6. Click **Activate**.
7. Enter the world.

If it does not appear, your folder is probably nested too deep.
Make sure `manifest.json` is directly inside the folder you copied.

---

## Use the item in-game

Run this command:

```mcfunction
/give @s bedrockmod:warp_relic
```

Hold the item in your main hand or offhand to teleport to:

`8000 75 8000`

---

## Files
- `manifest.json` - pack metadata.
- `items/warp_relic.json` - custom give-only item definition.
- `functions/tick.json` + `functions/tick.mcfunction` - teleports holders each tick.
