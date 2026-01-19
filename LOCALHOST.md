# How to Serve on Localhost

## Option 1: Python (Recommended - Simplest)

### Python 3.x
```bash
python -m http.server 8000
```
Or specify a port:
```bash
python -m http.server 3000
```

### Python 2.x
```bash
python -m SimpleHTTPServer 8000
```

Then open: **http://localhost:8000**

---

## Option 2: Node.js (http-server)

Install globally (one-time only):
```bash
npm install -g http-server
```

Run in your project directory:
```bash
http-server
```

Or specify a port:
```bash
http-server -p 3000
```

Then open: **http://localhost:8080** (or your specified port)

---

## Option 3: Node.js (Live Server)

Install globally:
```bash
npm install -g live-server
```

Run in your project directory:
```bash
live-server
```

Auto-opens browser at: **http://127.0.0.1:8080**

*Bonus: Auto-reloads on file changes!*

---

## Option 4: VS Code Live Server Extension

1. Install the "Live Server" extension by Ritwick Dey
2. Right-click `index.html` 
3. Select "Open with Live Server"
4. Auto-opens at: **http://127.0.0.1:5500**

---

## Option 5: PHP (If installed)

```bash
php -S localhost:8000
```

Then open: **http://localhost:8000**

---

## Testing Tips

### Desktop Testing
- Open DevTools (F12)
- Toggle device toolbar (Ctrl+Shift+M) to mobile view
- Test on different screen sizes

### Mobile Testing (Local Network)
```bash
# Find your computer's IP:
ipconfig getifaddr en0           # macOS
hostname -I | awk '{print $1}'   # Linux
ipconfig                          # Windows (find IPv4 Address)
```

Then on your phone, visit: **http://YOUR_IP:8000**

### Debugging
- Open DevTools Console (F12 → Console tab)
- Check for any errors
- Verify PIN entry works (PIN: 000000)

---

## Recommended Setup for Development

### Quick Start (Python)
```bash
cd c:/Users/HP/Desktop/Projects/RevolutPro
python -m http.server 8000
```

### Persistent Server (Node.js)
```bash
npm install -g live-server
cd c:/Users/HP/Desktop/Projects/RevolutPro
live-server --port=3000
```

Then visit: **http://localhost:3000**

---

## Troubleshooting

**Port already in use?**
```bash
# Use different port
python -m http.server 9000
```

**Permission denied?**
```bash
# Add sudo (Linux/Mac)
sudo python -m http.server 80
```

**Can't access from phone?**
- Ensure phone and computer are on same WiFi
- Check firewall settings
- Use the computer's local IP address (not 127.0.0.1)

---

## Test Features

Once running, test these flows:
1. **Login**: Enter phone number (e.g., 7700900000) → Continue
2. **PIN**: Enter 000000 → Sign In
3. **Dashboard**: Explore cards, balance, quick actions
4. **Transactions**: Search & filter transactions
5. **Navigation**: Bottom nav tabs are fully functional

Enjoy! 🚀
