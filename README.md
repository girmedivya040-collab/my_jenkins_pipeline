# Initialize Node project
npm init -y

# Install express
npm install express

# Create server.js
cat > server.js << 'EOF'
const express = require('express');
const app = express();
const path = require('path');

app.use(express.static(path.join(__dirname)));

const PORT = 3000;
app.listen(PORT, () => {
  console.log(`Server running on http://localhost:${PORT}`);
});
EOF

# Create README.md
cat > README.md << 'EOF'
# 🌐 Static Website Project

This is a simple static website built using:

- HTML
- CSS
- JavaScript
- Node.js (for local server)

---

## 🚀 How to Run

### Install dependencies
npm install

### Start server
node server.js

Open in browser:
http://localhost:3000

---

## 📁 Project Structure

index.html  
style.css  
script.js  
server.js  
package.json  
README.md  

---

## 👩‍💻 Author
Divya Girme
EOF
