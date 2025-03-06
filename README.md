# UIU-RP

The **UIU Research Portal (UIURP)** is a web-based platform designed to facilitate and promote research activities at United International University (UIU). It serves as a hub where students and faculty members can explore research projects, connect with mentors, and collaborate on academic initiatives. The portal provides essential features such as research project listings, faculty profiles, keyword-based search functionality, and a discussion forum to enhance engagement within the university's research community. 

---

## **Windows Setup**

### **1. Install MongoDB Community Edition**

1. **Download MongoDB**:

   - Visit the official MongoDB download page: [MongoDB Download Center](https://www.mongodb.com/try/download/community).
   - Select **Windows** as the operating system.
   - Choose the **MSI Installer** (easier installation).
   - Click **Download**.

2. **Run the Installer**:

   - Double-click the downloaded **MSI** file.
   - Follow the installation wizard:
     - Choose **Complete** installation.
     - Ensure **Install MongoDB as a Service** is checked.
     - Leave the default port **27017** (or change if necessary).
   - Click **Install** and complete the setup.

3. **Verify Installation**:

   - Open **Command Prompt** (`Win + R` → type `cmd` → press Enter).
   - Run the following command to check if MongoDB is installed:
     ```bash
     mongod --version
     ```
   - If the command works, MongoDB is installed successfully.

4. **Start MongoDB Service**:

   - Open **Command Prompt** and run:
     ```bash
     net start MongoDB
     ```
   - MongoDB should now be running on your system.

---

### **2. Install MongoDB Compass (GUI Tool)**

1. **Download MongoDB Compass**:

   - Visit the official download page: [MongoDB Compass Download](https://www.mongodb.com/products/compass).
   - Select **Windows** and download the installer.

2. **Run the Installer**:

   - Double-click the installer and follow the setup instructions.

3. **Connect MongoDB Compass to Local MongoDB Server**:

   - Open **MongoDB Compass**.
   - In the **Connection** field, enter:
     ```
     mongodb://localhost:27017
     ```
   - Click **Connect**.
   - You should now see the databases and collections.

---

## **macOS Setup**

### **1. Install MongoDB Community Edition**

MongoDB is installed on macOS via **Homebrew**.

1. **Install Homebrew** (if not already installed):

   - Open **Terminal** and run:
     ```bash
     /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
     ```

2. **Install MongoDB**:

   - Run the following command:
     ```bash
     brew tap mongodb/brew
     brew install mongodb-community@7.0
     ```
   - Replace `7.0` with the latest MongoDB version if needed.

3. **Start MongoDB Service**:

   - Run:
     ```bash
     brew services start mongodb-community@7.0
     ```

4. **Verify Installation**:

   - Run:
     ```bash
     mongod --version
     ```
   - If it returns a version number, MongoDB is installed successfully.

---

### **2. Install MongoDB Compass**

1. **Download MongoDB Compass**:

   - Visit: [MongoDB Compass Download](https://www.mongodb.com/products/compass).
   - Select **macOS** and download the `.dmg` file.

2. **Install MongoDB Compass**:

   - Open the **.dmg** file.
   - Drag the **MongoDB Compass** icon to the **Applications** folder.

3. **Connect MongoDB Compass to Local MongoDB Server**:

   - Open **MongoDB Compass**.
   - In the **Connection** field, enter:
     ```
     mongodb://localhost:27017
     ```
   - Click **Connect**.
   - You should now see your MongoDB databases.

---

## **Additional Commands**

### **Starting MongoDB Manually**

If MongoDB is not running, start it manually:

- **Windows**:
  ```bash
  net start MongoDB
  ```
- **macOS**:
  ```bash
  brew services start mongodb-community@7.0
  ```

### **Stopping MongoDB**

- **Windows**:
  ```bash
  net stop MongoDB
  ```
- **macOS**:
  ```bash
  brew services stop mongodb-community@7.0
  ```

### **Accessing the MongoDB Shell**

To enter the MongoDB shell:

```bash
mongosh
```

---

## **Conclusion**

Now you have **MongoDB** installed and running, along with **MongoDB Compass** for database management. Let me know if you need help with further configurations! 🚀
