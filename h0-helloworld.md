# h0 

## 1) Ohjelman kirjoitus
Tein helpon "Hello world"-ohjelman jonka tekoon löytyi useita esimerkkejä. 

     $ #include <iostream>

     int main() {
     std::cout << "Hello world!" << std::endl;
     return 0;
     }

Ohjelma on kirjoitettu  Linuxin virtuaalikoneessa Nano-editorilla c++-kielellä. Minulla ei ole aiempaa kokemusta C tai C++ ohjelmoinnista. Ensimmäinen yritys VS Codella ja Pythonilla ei onnistunut, Linux vaikuttaa toimivammalta ympäristöltä.

## 2) Ohjelman kääntäminen

     g++ Helloworld.cpp -o helloworld.exe
     
     ./helloworld.exe suorittaa käännetyn ohjelman.
    
Ohjelman kääntämiseen sai selkeät ohjeet ChatGPT:lta. Käytössäni on sen ilmaisversio (kielimalli GPT-5.6 Luna, oletusasetuksilla) . Ohjelman kääntämiseen binääriksi käytin g++ kääntäjää. 

## 3) Binäärin analysointi

Tietoja ohjelmasta pääsee katsomaan useilla komennoilla.

    -file helloworld.exe kertoo esimerkiksi "ELF 64-bit LSB pie executable"
    -readelf -h helloworld.exe-komennolla saa tietoa esimerkiksi ohjelman versioista ja tyypistä
    -komentorivin työkalulla hexdump, voidaan tutkia binaaritiedoston sisältöä heksadesimaali-, desimaali-, oktaali- tai ASCII-muodossa

## Lähteet
C++ "Hello, World!" Program, https://www.programiz.com/cpp-programming/examples/print-sentence 

Hexdump, Hexdump command in Linux with examples https://www.geeksforgeeks.org/linux-unix/hexdump-command-in-linux-with-examples/ 

Hexdump, Linux manual page https://man7.org/linux/man-pages/man1/hexdump.1.html 


