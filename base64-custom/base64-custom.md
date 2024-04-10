# base64-custom THCON 2024

### Note:- My solution is little bit lengthy because i was away from my laptop and did this challenge on paper using pencil i.e. manually.

## Challenge
![Challenge](https://2-quantum.github.io/THCON-2k24/base64-custom/base64-ques.png)

## Understanding the challenge

### How base64 works
1. It takes every single letter of the word.
2. Then it converts it into decimal.
3. Then the decimal is converted into binary having length 8 bits.
4. Then the binary is regrouped with every binary having length of 6 bits.
5. Then the binary is converted into decimal.
6. Then the decimal is converted into another character according to base64 index table.

![base64-index-table](https://2-quantum.github.io/THCON-2k24/base64-custom/base64-index-table.jpeg)

### What is different in this base64custom
- It is told that sextets are changed into quintuplets which means in the 4th step instead of 6 bits the length was 5 bits.

### Contents of message.txt
```
KREEGTaOPNRDIcbFGYaFeMLTLcaHOMbTGBWWKXbJNZXGSdDd
```
### Reversing the process to obtain flag
![process](https://2-quantum.github.io/THCON-2k24/base64-custom/base64-1.jpeg)
- Instead of word it will be decimal in 1st step.
- message.txt contains 48 letters and i divided them into group of 8 because those 8 letters will give 40 bits (8×5 bits) and from those 40 bits 5 letters will be formed (5×8 bits).

### Solution
![step-1](https://2-quantum.github.io/THCON-2k24/base64-custom/base64-2.jpeg)
![step-2](https://2-quantum.github.io/THCON-2k24/base64-custom/base64-3.jpeg)
![step-3](https://2-quantum.github.io/THCON-2k24/base64-custom/base64-4.jpeg)
![step-4](https://2-quantum.github.io/THCON-2k24/base64-custom/base64-5.jpeg)
