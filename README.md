# CODECRAFT_CS_01
Task 01: Implement Ceaser Cipher
1. Understanding the Ceaser Cipher
     - The Caesar cipher shifts each letter in the plaintext by a fixed number of     
     positions.
     - For example, with a shift of 3:
       ABC => DEF

2. Choose the shift(key)
     - The "key" in a Caesar cipher is the number of positions by which each letter will be shifted in the alphabet.
     - For example:\
  If the key is 3, then A will become D, B will become E, and so on.\
  If the key is 13, then A will become N, B will become O, etc.

3. Writing the Algorithm
     - Encryption Algorithm:\
         For each letter in the plaintext:\
         If it's a letter, shift it by the key.\
         If it's not a letter (like a space or punctuation), leave it unchanged.\
         Wrap around the alphabet if the shift goes past Z or z
     - Decryption Algorithm:\
         The decryption is the reverse process, where each letter is shifted by the negative of the key (i.e., left by the same amount).

4. Edge Cases to Consider
     - Non-alphabetical characters: Spaces, punctuation, and numbers should remain unchanged in the encryption and decryption process.
     - Negative shift: The shift can be negative for decryption, or if you want to apply a reverse shift (e.g., shift = -3 for encryption).

5. Optimizations and Enhancements
     - Case-insensitive encryption: If you want to ignore case and treat all letters as the same, adjust your code to handle both cases uniformly.
     - Unicode support: This basic Caesar cipher only works for English letters. To support other languages or Unicode characters, you would need to adjust the algorithm. 
