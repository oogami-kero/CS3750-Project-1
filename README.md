# CS3750-Project-1
Project for Computer and Network Security Class

Demonstration of application of RSA, AES, and SHA256 encryption algorithms for confidentiality purposes, for a sender then the decryption of the file for a receiver. 

    Generate the symmetric, public, and private key's for the sender and receiver in using the KeyGen.java file in the KeyGen directory.

cd .\KeyGen\
javac KeyGen.java
java KeyGen

    Then it prompts the user to generate a 16 character symmetric.key, such as:

1234567890abcdef

    The Sender is using encryption algorithm RSA-En Ky+ (AES-En Kxy (SHA256 (M)) || M) and the Receiver uses an opposite algorithm
    Copy the keys into the correct directories from the KeyGen directory:

cp .\symmetric.key ..\Sender\
cp .\symmetric.key ..\Receiver\
cp .\YPublic.key ..\Sender\
cp .\YPrivate.key ..\Receiver\

    Compile and run the Sender.java file and once prompted, enter in the example file

cd ..\Sender\
javac Sender.java
java Sender

    Three files that will have been created:

    message.dd
    message.add-msg 
    message.rsacipher

    Compile and run the Receiver.java file and enter the file to put the decrypted message in file:

cd ..\Receiver\
javac Receiver.java
java Receiver

    Once ran, and input of a decrypted file has been entered, you should have these new files in your Receiver directory:

    aesTemp.dd
    garden-decrypted.tx
    message.add-msg
    message.dd
