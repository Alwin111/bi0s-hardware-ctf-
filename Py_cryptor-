# Py_cryptor-
bi0s hardware -ctf

The task was to run the python code.But since the chal.pyc file was compiled file 
pyc file means it is a compiled output file generated from source code written in Python programming language.
so to open it we need to use a decompiler and i searched for a pyc file decompiler and found one and
decompiled it. And ater decompiling it i got a python code and the password was already given 
so i need to reverse it so i copy pasted the python code and password into chatgpt and ask it 
find the pathway that leads to the password and it modified the python code so i copyed the python code
and used python online compiler to run the code and i got the flag
def decrypt_xor(text):
    return ''.join(chr(ord(c) ^ 14) for c in text)

def decrypt_caesar(text, shift):
    decrypted_text = ''
    for c in text:
        if c.isupper():
            decrypted_text += chr((ord(c) - shift - 65) % 26 + 65)
        elif c.islower():
            decrypted_text += chr((ord(c) - shift - 97) % 26 + 97)
        else:
            decrypted_text += c
    return decrypted_text

# Given encrypted string
encrypted_string = "w:~=Qwc=Qy?v^Ql?}Q`w"

# Step 1: XOR decryption with key 14
xor_decrypted = decrypt_xor(encrypted_string)

# Step 2: Caesar cipher decryption with shift 5
caesar_decrypted = decrypt_caesar(xor_decrypted, 5)

print(caesar_decrypted)

the flag is =wired{t4k3_th3_r1sK_w1n_it}
