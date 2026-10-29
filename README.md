```
# ✨ Discord Humanizer

**Bulk Discord Profile Customizer**  
Make your accounts look human — fast, clean, and effortless.

A powerful multi-threaded tool designed for mass profile customization.  
Change display names, bios, pronouns, avatars, and HypeSquad houses with full proxy support and automatic retry system.

---

## 🚀 Features

- 🎲 **Random Display Names** – Pulls from your custom name list  
- 📝 **Random Bios** – Fresh status every time  
- 🏷️ **Random Pronouns** – Fully customizable  
- 🖼️ **Avatar Changer** – Supports PNG, JPG, GIF & WebP  
- 🏠 **HypeSquad Changer** – Random house assignment  
- 🌐 **Proxy Support** – HTTP / SOCKS with authentication  
- ⚡ **Multi-threaded** – Process hundreds of tokens simultaneously  
- 🔄 **Auto Retry System** – Never lose progress on temporary failures  
- 📂 **Smart Token Sorting** – Success & failed tokens automatically separated  
- 🔧 **Dynamic Discord Build Fetch** – Always uses the latest Discord client build  
- 🧹 **Clean Console Logs** – Beautiful, readable output  

---

## 📦 Setup

### 1. Install Python
Download **Python 3.11+** from:  
[https://www.python.org/downloads/](https://www.python.org/downloads/)

✅ Make sure to check **"Add Python to PATH"** during installation.

### 2. Install Dependencies
Open terminal in the project folder and run:

```bash
pip install -r req.txt
```

Or simply start the tool — it will install missing packages automatically:

```bash
python main.py
```

---

## 📁 Folder Structure

```text
Discord Humanizer/
├── data/
│   ├── bios.txt
│   ├── names.txt
│   └── pronouns.txt
├── input/
│   ├── tokens.txt
│   ├── proxies.txt
│   ├── success.txt
│   └── failed.txt
├── avatar/
│   ├── avatar1.png
│   ├── avatar2.jpg
│   └── ...
├── config.json
└── main.py
```

---

## 📄 Input Files

### `tokens.txt`
One token per line:

```text
MTQx....token1
MTQx....token2
MTQx....token3
```

### `proxies.txt`
Supported formats:

```text
ip:port
ip:port:user:pass
user:pass@ip:port
http://user:pass@ip:port
```

Leave the file empty if you don’t want to use proxies.

### `names.txt`
```text
zenkai
akira
ghost
midnight
```

### `bios.txt`
```text
sleeping
touching grass
idk anymore
just vibing
```

### `pronouns.txt`
```text
he/him
she/her
they/them
any/all
```

---

## ⚙️ Configuration

Edit `config.json` to control what gets changed:

```json
{
  "max_threads": 3,
  "avatar_dimension": 256,
  "max_avatar_cache": 100,
  "update_display_name": true,
  "update_bio": true,
  "update_pronouns": true,
  "update_avatar": true,
  "update_hypesquad": true,
  "RetryLimit": 1
}
```

---

## ▶️ How to Run

```bash
python main.py
```

You will be prompted for the number of threads when starting.

---

## 📊 Results

| Status       | File Location          |
|--------------|------------------------|
| Successful   | `input/success.txt`    |
| Failed       | `input/failed.txt`     |

Processed tokens are automatically removed from `tokens.txt`.

---

## 💡 Pro Tips

- Use high-quality residential or mobile proxies for best results  
- Large avatars are automatically compressed  
- Bad proxies are detected and removed  
- Duplicate tokens are ignored  
- PNG / JPG / GIF / WebP avatars are fully supported  

---

## 📋 Requirements

- Python **3.11+**
- Windows recommended (works on other OS too)

---

## 👨‍💻 Credits

**Developer:** zoro

---

> Made with ❤️ for clean and natural Discord accounts
```
