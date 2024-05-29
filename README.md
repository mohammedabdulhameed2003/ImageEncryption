# ImageEncryption
The "Multiple Image Encryption" app uses Streamlit to provide a user-friendly interface for securely encrypting and decrypting images. It leverages advanced cryptographic techniques, including 3D sine chaos systems and DNA-RNA-based algorithms, to enhance the security of image data.
![Screenshot (33)](https://github.com/mohammedabdulhameed2003/ImageEncryption/assets/135050083/a2f132d3-4b9d-4b6c-b727-f37fcaa1ff26)
![Screenshot (35)](https://github.com/mohammedabdulhameed2003/ImageEncryption/assets/135050083/c3d6b155-dd12-45b1-a8f0-047c95973639)
Multiple Image Encryption App
Overview
The "Multiple Image Encryption" app uses Streamlit to provide a user-friendly interface for securely encrypting and decrypting images. It leverages advanced cryptographic techniques, including 3D sine chaos systems and DNA-RNA-based algorithms, to enhance the security of image data.

Features
Multiple Image Upload:

Users can upload multiple images simultaneously.
Supports image formats like JPG, JPEG, and PNG.
Images must be either 256x256 or 512x512 pixels in dimension.
Image Canvas Creation:

Images are organized on canvases based on their dimensions:
512x512 images are placed on individual canvases.
256x256 images are combined into a single canvas, with up to four images per canvas.
Image Display:

Uploaded images are displayed on the app interface for visual confirmation.
The app indicates the number of uploaded images.
Encryption and Decryption:

A button triggers the encryption and decryption processes.
Uses a combination of SHA-256, 3D sine chaos systems, and DNA-RNA encryption techniques.
The encrypted and decrypted images are displayed in a side-by-side comparison.
Encryption Process
SHA-256 Hashing:

Computes a SHA-256 hash of the image data, converting it into a 256-bit binary string.
Intermediate Parameter Calculation:

Uses hash values and external keys to compute intermediate parameters (h1 to h6).
Initial Values and Chaotic Parameters:

Derives initial values (x0, y0, z0, p0, q0) for the chaotic system based on intermediate parameters.
Calculates chaotic system parameters (a, b, c, d).
3D Sine Chaos System:

Generates chaotic sequences (X1, X2, X3) used for image scrambling.
DNA Encoding:

Converts the bit-plane representation of the image into a DNA sequence based on predefined encoding rules.
RNA Transcription:

Transcribes the DNA sequence into RNA.
Mutation and Translation:

Applies mutation rules to the RNA sequence.
Translates the mutated RNA sequence back to DNA.
RNA Encoding:

Encodes the translated DNA sequence into a final RNA sequence using chaotic sequences.
RNA Computing:

Computes the final encrypted matrix using XOR operations based on RNA encoding rules.
Binary Matrix to Decimal:

Converts the binary matrix of the encrypted image back into a decimal format for display.
Decryption Process
RNA Computing Reverse:

Reverses the RNA computing process to retrieve the initial encoded matrix.
Reverse RNA Translation:

Translates the RNA sequence back to its original DNA form.
Reverse RNA Mutation:

Applies reverse mutation rules to get back the initial RNA sequence.
Reverse Transcription:

Transcribes the RNA sequence back to DNA.
DNA Decoding:

Decodes the DNA sequence back to its original binary format.
Reconstruct Image:

Converts the binary matrix back to image pixels, reconstructing the original image.
Visualization
Displays encrypted and decrypted images side by side for visual comparison.
Utilizes Matplotlib for plotting images within the Streamlit interface.
Usage
Upload Images: Use the file uploader to select and upload images.
View Uploaded Images: The app displays the uploaded images and the number of images uploaded.
Encrypt and Decrypt: Click the "Encrypt and Decrypt Images" button to process the images. The encrypted and decrypted images are then displayed.
This app provides a secure and sophisticated method for encrypting and decrypting image data, making it suitable for applications requiring high levels of data protection.
