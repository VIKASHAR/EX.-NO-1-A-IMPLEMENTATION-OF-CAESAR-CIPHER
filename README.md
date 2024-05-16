# EX. NO: 1(A) : IMPLEMENTATION OF CAESAR CIPHER

## AIM:
To implement the simple substitution technique named Caesar cipher using python language.

## ALOGORITHM:

STEP-1: Read the plain text from the user.

STEP-2: Read the key value from the user.

STEP-3: If the key is positive then encrypt the text by adding the key with each character in the plain text.

STEP-4: Else subtract the key from the plain text.

STEP-5: Display the cipher text obtained above.

## PROGRAM:

  '''python
  #A python program to illustrate Caesar Cipher Technique
  def encrypt(text,s):
  	result = ""
  
  	# traverse text
  	for i in range(len(text)):
  		char = text[i]
  
  		# Encrypt uppercase characters
  		if (char.isupper()):
  			result += chr((ord(char) + s-65) % 26 + 65)
  
  		# Encrypt lowercase characters
  		else:
  			result += chr((ord(char) + s - 97) % 26 + 97)
  
  	return result
  
  #check the above function
  text = "ATTACKATONCE"
  s = 4
  print ("Text : " + text)
  print ("Shift : " + str(s))
  print ("Cipher: " + encrypt(text,s))
'''

## OUTPUT:

![image](https://github.com/VIKASHAR/EX.-NO-1-A-IMPLEMENTATION-OF-CAESAR-CIPHER/assets/119405655/7b57b7a4-29e5-4a87-a9f2-26d786e42eec)


## RESULT :
 Thus the implementation of ceasar cipher had been executed successfully.
