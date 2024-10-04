# base64-custom THCON 2024

## Challenge
![Challenge](base64-ques.png)

## Understanding the challenge

### How base64 works
1. It takes every single letter of the word.
2. Then it converts it into decimal.
3. Then the decimal is converted into binary having length 8 bits.
4. Then the binary is regrouped with every binary having length of 6 bits.
5. Then the binary is converted into decimal.
6. Then the decimal is converted into another character according to base64 index table.

![base64-index-table](base64-index-table.jpeg)

### What is different in this base64custom
- It is told that sextets are changed into quintuplets which means in the 4th step instead of 6 bits the length was 5 bits.

### Contents of message.txt
```
KREEGTaOPNRDIcbFGYaFeMLTLcaHOMbTGBWWKXbJNZXGSdDd
```

## Solution
- It is same as base32 but with a condition that all the alphabets will be according to base64.
![b321](b321.png)
![b322](b322.png)
