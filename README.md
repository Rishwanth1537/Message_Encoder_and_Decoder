# Message_Encoder_and_Decoder
🔐 Secret Message Encoder and Decoder with GUI (Python + Tkinter)
This Python application allows users to encrypt and decrypt messages using a simple character substitution cipher. It provides a clean graphical user interface (GUI) built with Tkinter, where users can input a message, encrypt or decrypt it, and view the result.

💡 How It Works:
Character Mapping:
The program creates two character sets:
a: A list containing all printable characters (space, punctuation, letters, and digits).
b: A shuffled copy of a used for encoding.
This shuffled version (b) acts as the cipher key, mapping each character in a to a different one in b.

Encryption:
Each character in the input message is replaced with the corresponding character in the shuffled list b. If a character isn't found in the original list (e.g., emojis or special characters), it's added unchanged.
Decryption:
Reverses the process by finding each encrypted character's position in the shuffled list b and replacing it with the corresponding character from the original list a.

🖥 GUI Features:
Input Field: Type the message to be encoded or decoded.
Encrypt Button: Encrypts the message using the random character mapping.
Decrypt Button: Decrypts the message back to its original form (only if the same mapping is used).
Output Field: Displays the result of the encryption or decryption.

⚠️ Important Note:
The mapping (a and shuffled b) is generated every time the script runs, so:
Decryption will only work if the encrypted message is decoded during the same session.
To maintain consistent decoding, you'd need to save the key (b) when encrypting and reuse it during decryption.

