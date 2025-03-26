## **MERN Stack Installation Guide**

### **1. Install VS Code**

1. Go to [https://code.visualstudio.com](https://code.visualstudio.com)
2. Download the installer for your OS (Windows, macOS, Linux)
3. Run the installer and follow the on-screen instructions
4. After installation, open VS Code
5. (Optional) Install the following extensions:
   - **ES7+ React/Redux/React-Native snippets**
   - **Prettier – Code Formatter**
   - **REST Client**

---

### **2. Install Node.js**

1. Go to [https://nodejs.org](https://nodejs.org)
2. Download the **LTS (Long-Term Support)** version for your OS
3. Run the installer:
   - Accept the license agreement
   - Keep the default installation options
4. After installation, verify using the terminal:

```bash
node -v
npm -v
```

5. Update npm (if needed):

```bash
npm install -g npm
```

---

### **3. Install MongoDB**

#### ➡️ Option 1: Install MongoDB Community Edition (Local)

1. Go to [https://www.mongodb.com/try/download/community](https://www.mongodb.com/try/download/community)
2. Download the installer for your OS
3. Follow the on-screen instructions (choose the default settings)
4. Start MongoDB server:

```bash
mongod
```

5. Verify MongoDB is running:

```bash
mongo
```

#### ➡️ Option 2: Use MongoDB Atlas (Cloud)

1. Go to [https://www.mongodb.com/cloud](https://www.mongodb.com/cloud)
2. Create an account
3. Create a cluster
4. Get the connection string and connect using Mongoose

---

### **4. Install Git**

1. Go to [https://git-scm.com](https://git-scm.com)
2. Download the installer for your OS
3. Follow the default installation settings
4. Verify installation:

```bash
git --version
```

---

### **5. Install React**

1. Create a new React project:

```bash
npx create-react-app my-mern-app
```

2. Navigate to the project folder:

```bash
cd my-mern-app
```

3. Install dependencies:

```bash
npm install
```

4. Start the React development server:

```bash
npm run dev
```

---

### **6. Install Express.js**

1. Create a `server` folder in your project
2. Install Express.js:

```bash
npm install express
```

3. Create `server.js`:

```javascript
const express = require('express');
const app = express();
const PORT = 5000;

app.get('/', (req, res) => {
    res.send('API is working');
});

app.listen(PORT, () => console.log(`Server running on port ${PORT}`));
```

4. Start the server:

```bash
node server.js
```

---

### **7. Install Mongoose**

1. Install Mongoose:

```bash
npm install mongoose
```

2. Connect MongoDB in `server.js`:

```javascript
const mongoose = require('mongoose');

mongoose.connect('mongodb://localhost:27017/myapp', {
  useNewUrlParser: true,
  useUnifiedTopology: true,
}).then(() => console.log('MongoDB connected'))
  .catch(err => console.log(err));
```

---

### **8. Install Postman (Optional)**

1. Go to [https://www.postman.com](https://www.postman.com)
2. Download and install the application
3. Use Postman to test your backend APIs

---

### **9. Install React Developer Tools (Optional)**

1. Open Google Chrome
2. Go to the Chrome Web Store
3. Search for **React Developer Tools**
4. Click **Add to Chrome**

---

### ✅ **Your MERN stack environment is now ready!**

