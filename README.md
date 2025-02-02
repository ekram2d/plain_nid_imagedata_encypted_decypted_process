# Secure ID Card Processing with Encryption

This project extracts an ID number from an image using OCR, encrypts it using AES-256, modifies the image to mask the ID, and allows decryption to restore the original ID.

## Features
- Extracts ID number from an image using EasyOCR
- Encrypts the ID number using AES-256 (Fernet encryption)
- Replaces the ID number in the image with an encrypted version
- Allows decryption and restoration of the original ID number
- Saves original, modified, and restored images
- Provides visualization of the encryption and decryption process

## Prerequisites
Make sure you have Python installed on your system (Python 3.7 or later).

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/secure-id-encryption.git
   cd secure-id-encryption
   ```

2. Install required dependencies:
   ```sh
   pip install -r requirements.txt
   ```
   If you don’t have a `requirements.txt`, install manually:
   ```sh
   pip install easyocr pillow cryptography numpy matplotlib
   ```

3. Ensure you have the necessary OCR language model downloaded when running the script for the first time.

## Usage

1. Place your ID card image in the project folder.
2. Update the `image_path` variable in `incrypted_decrypted.py` with your image path.
3. Run the script:
   ```sh
   python incrypted_decrypted.py
   ```

## Expected Output
- The script processes the ID image, encrypts the ID number, and saves three images:
  - `original_id_card.jpg`: The original ID card image
  - `modified_id_card.jpg`: The image with the ID number masked
  - `decrypted_id_card.jpg`: The restored image with the original ID visible
- It also displays the processed images with matplotlib visualization.

## Notes
- If you are using Google Colab, ensure your image is uploaded, and adjust the file path accordingly.
- The script downloads the processed images automatically in Google Colab.
- If you encounter font issues, install the DejaVu font or use the default system font.

## License
This project is open-source under the MIT License.

﻿# plain_nid_imagedata_encypted_decypted_process
