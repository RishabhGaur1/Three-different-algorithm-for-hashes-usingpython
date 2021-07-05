# Three-different-algorithm-for-hashes-usingpython

#Algorithm 1

import hashlib
print('\SHA256')

#initialising input data 
m = hashlib.sha256()
m.update(b"initialising")
m.update(b"User")

#generating hashes 

print('Your Output 1 :', m.digest())
x = hashlib.sha256(b"User 2 initialising ")
print('Your Output 2 :', x.digest())


#Algorithm 2

import hashlib
print('\SHA384')

#initialising input 
m = hashlib.sha384()
m.update(b"initialising")
m.update(b"User")

#generating hashes of input value
print('Output 1 :', m.digest())
x = hashlib.sha384(b"User2 initialising")
print('Output 2 :', x.digest())




#Algorithm 3
import hashlib
print('\ blake2b' )

#initialising input
m = hashlib.blake2b()
m.update(b"initialising")
m.update(b"User")

#generating hashes of input values
print('Output 1 :', m.digest())
x = hashlib.blake2b(b"User2 initialising")
print('Output 2 :', x.digest())
