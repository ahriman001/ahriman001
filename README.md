https://rubika.ir/icubjjc
for word in pass_file:
    enc_word = word.encode('utf-8')
    hash_word = hashlib.md5(enc_word.strip())
    digest = hash_word.hexdigest()
    if digest == input_hash:
        print("Password found.\nThe password is:", word)
        pass_found = 1
        break
      
