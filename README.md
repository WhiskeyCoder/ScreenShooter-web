## 🖥️ ScreenShooter_web.py

**Automatically screenshot websites from a list.**

Give it a list of URLs, and this script will open each one and save a full-page screenshot into a `/shots/` folder. Great for archiving, research, visual monitoring, or just seeing who's still alive on the internet.

---

### 🌐 What It Does

- Reads a list of domain names or URLs from a `websites.txt` file
- Uses **Selenium** and **Chrome WebDriver** to open each site
- Waits 3 seconds to ensure the page loads
- Saves a screenshot of each page in the `./shots/` directory

---

### 📁 Folder Structure
```
project-folder/
├── ScreenShooter_web.py
├── websites.txt          # <-- List of domains (e.g., example.com)
└── shots/                # <-- Output folder for PNG screenshots
```

---

### 🧰 Requirements

- Python 3.x
- `selenium`
- `webdriver-manager`

Install them with pip:
```bash
pip install selenium webdriver-manager
```

---

### 📝 How To Use

1. Create a text file named `websites.txt`
    ```
    example.com
    github.com
    wikipedia.org
    ```

2. Run the script:
```bash
python ScreenShooter_web.py
```

3. Screenshots will be saved into the `/shots/` folder.

---

### ⚠️ Notes

- Make sure `/shots/` exists before running the script, or it may fail.
- URLs are prefixed with `https://` by default. If the site is HTTP-only, adjust the script.
- Bad or non-screenshotable sites are gracefully skipped with an error message.
- Chrome browser must be installed.

---

### 💡 Example Output
```
capturing example.com
capturing github.com
capturing wikipedia.org
wobblyweirdwebsite.biz not scrapabale
```

---

### 🧙‍♂️ Author
By [WhiskeyCoder](https://github.com/WhiskeyCoder), who firmly believes screenshots are forever.

---

### 📜 License
MIT — because if it works, let the people use it.

