# 🧅 KodeKTep - Encryption

> "Not everything that looks like a PDF is just a document."

**KodeKTep** is a file encryption and stealth packaging tool. Created for those who value true privacy, digital disguise, and content security.

---

## 🔐 What does KodeKTep do?

- Encrypts the **contents of any file** (text, image, spreadsheet, code, etc.)
- Merges the encrypted result into a **base file** (like a PDF, image, or executable)
- Produces a **perfectly functional file** that appears normal but contains hidden content
- Generates a `.keys` file containing the decryption metadata, **essential for recovering the original content**

With this, you can hide:
- An executable inside an image
- A video inside a `.txt` file
- A secret document inside another PDF
- Or even a photo inside another photo—keeping the host file fully operational

---

## 📦 What does this repository contain?

At this stage, we're releasing only the **Windows executable** (`kodektep.exe`). Future versions for Linux, macOS, and CLI will be added soon.

---

## 🚀 How to use

### 🧪 Encrypting a file

1. Run `kodektep.exe`
2. Select mode: **Encrypt**
3. Choose the **file you want to protect** (e.g., `image.jpg`)
4. (Optional) Select a **base file** (e.g., `document.pdf`) to host the hidden data
5. Click **Run**
6. The program will generate:
   - A new file with `_oc` suffix (e.g., `document_oc.pdf`)
   - A `.keys` file (e.g., `document_oc.pdf.keys`) essential for decryption

> If no base is used, the output file will have the `.ocpher` extension

---

### 🧹 Decrypting a file

1. Run `kodektep.exe` again
2. Select mode: **Decrypt**
3. Choose the previously generated file (e.g., `document_oc.pdf`)
4. Ensure the corresponding `.keys` file is in the **same folder** with the **same base name**
5. Click **Run**
6. The original file will be restored with its name + `+KodeKTep` (e.g., `image+KodeKTep.jpg`)

---

## 🛡 About security

- Without the `.keys` file, **decryption is mathematically infeasible**
- Each operation generates **unique and random AES keys and IVs**
- The final file is **fully functional** (opens like a normal file) but secretly contains hidden data

---

## 📌 Important Notes

- The project is **not yet open-source**, but partial release may happen later
- Your security depends on the **preservation of the `.keys` file**. If lost, the content is **irretrievable**

---

## 📬 Contact

This project was created by **Paulo Sergio Durco** (@psdurco)

If you’d like to collaborate, test future versions, or support the project, feel free to open an issue or reach out (link coming soon).
