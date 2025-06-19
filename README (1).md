# 🔐 Steganography- Hiding Information in the Image( Using ASCII Technique)

This project implements a basic form of **image steganography** where a **text message is securely hidden within an image** by encoding the ASCII values of characters into the pixel values of the image. The encryption technique is simple XOR-based, and this solution demonstrates how digital images can be used for secure message transmission.

---

## 📌 Problem Statement

In a digital world where privacy and security are paramount, simply encrypting a message may not be enough. This project aims to **embed encrypted messages within images** using steganography techniques to hide the presence of the message itself.

---

## 🛠️ System Development Approach

- **Language:** Python  
- **Libraries Used:**
  - `OpenCV (cv2)` – for image processing
  - `NumPy` – for numerical manipulation

- **Concept Used:**
  - ASCII encoding of text
  - Simple XOR encryption with a key
  - Pixel-wise embedding into RGB channels

---

## 🧠 Algorithm & Deployment

### 🔐 **Encryption/Embedding:**
1. User inputs a message and a secret key.
2. Each character of the message is converted into its ASCII value.
3. The ASCII value is XORed with a key character.
4. The result is embedded into image pixel channels (`R`, `G`, `B`).
5. Save the modified image.

### 🔓 **Decryption/Extraction:**
1. Load the stego image.
2. Enter the same secret key.
3. Extract XORed ASCII values from pixels.
4. XOR them again with the key to get original characters.

---

## 📷 Result

- The original image remains visually unchanged.
- The hidden message is securely embedded.
- Only users with the correct key can recover the message.
- Wrong keys lead to garbage or unreadable output.

---

## 🧪 Sample Output

##Original Image


![Image](https://github.com/user-attachments/assets/ae15283c-4610-4112-be60-89a5408265c0)


##Encrypted Image


![Image](https://github.com/user-attachments/assets/117d0eff-18c6-4af6-88f3-6e3290ddb13f)


---

## ✅ Conclusion

- ASCII-based steganography offers a lightweight, secure method.
- Suitable for short messages and digital watermarking.
- No visible degradation of the image.
- Simple XOR logic makes it easy to implement and understand.

---

## 🚀 Future Scope

- Add AES/RSA encryption layer.
- Move to LSB-based embedding for better efficiency.
- Create a user-friendly GUI.
- Expand to audio/video steganography.

---

## 📚 References

- https://en.wikipedia.org/wiki/Steganography  
- https://docs.opencv.org/  
- https://numpy.org/  
- Jupyter Notebook: `Stegno_ascii technique.ipynb`  

---


