# Pudina Alena
# Contact Info
### **Email** 
* [gueguc@gmail.com](mailto:gueguc@gmail.com) 
* [morven2016@yandex.ru](mailto:morven2016@yandex.ru)
  
### Phone number
[+7(996) 963 - 29 - 46](tel:+79969632946)
### Telegram
[@AlenaPudina](https://t.me/AlenaPudina)
### VK
[https://vk.com/id54281260](https://vk.com/id54281260)
### Discord
[@alena077076](https://discordapp.com/users/1178825408997752894/)

# Summary

A responsible and challenge-ready person, interested in new things. I am used to dealing with large amounts of information and I know how to work in a team.

## Work experience

* *11/2021 - 10/2022* - Project Manager (Roskvartal)

    Duties:
    - Writing technical documentation
      + Writing technical specifications for concluding contracts with the customer
      + Forming tasks for developers in Trello
    - Developing prototypes of page layouts for setting a task for the designer
    - Maintaining project documentation in Bitbucket
    - Content and maintenance of websites:
        + Adding content via the administrative panel
        + Translation of site content into English
        + Formation of news content (selection of news)
    - Forming bug reports upon request from users or while working with the website

* *10/2022 - now* - Freelance

    - Developed websites on Wordpress and Tilda
    - Typeset collections with selections of scientific articles for publication
    - Creating chat-bots for Telegram
 
# Skills
* HTML
* CSS 
    + Vanilla CSS
    + BootStrap
* JavaScript
    + Vue
* Version control
    + Git
    + Bitbucket
* No-sciprt-constructor
    + Tilda
    + WordPress
* Python
    + NumPy
    + TensorFlow
* C++
    + Qt
* R, Maple, MathCAD
* Java

# Examples
## Task1
Given two sorted arrays nums1 and nums2 of size m and n respectively, return the median of the two sorted arrays.

The overall run time complexity should be O(log (m+n)).

```
class Solution:
    def findMedianSortedArrays(self, nums1: List[int], nums2: List[int]) -> float:
        l1, l2 = len(nums1), len(nums2)
        i1, i2 = 0, 0
        res = []
        while i1+i2 < l1 + l2 :
            if i2 == l2  or i1 < l1 and nums1[i1] <= nums2[i2]:
                res.append(nums1[i1])
                i1 += 1
            else:
                res.append(nums2[i2])
                i2 += 1

        if len(res) % 2 == 1:
            return res[len(res) // 2]
        else:
            return (res[len(res) // 2 - 1] + res[len(res) // 2]) / 2
        
```

## Task2

Seven different symbols represent Roman numerals with the following values:

|Symbol|	Value|
|-|-|
|I|	1|
|V	|5|
|X|	10|
|L|	50|
|C|	100|
|D	|500|
|M	|1000|

Roman numerals are formed by appending the conversions of decimal place values from highest to lowest. Converting a decimal place value into a Roman numeral has the following rules:

If the value does not start with 4 or 9, select the symbol of the maximal value that can be subtracted from the input, append that symbol to the result, subtract its value, and convert the remainder to a Roman numeral.
If the value starts with 4 or 9 use the subtractive form representing one symbol subtracted from the following symbol, for example, 4 is 1 (I) less than 5 (V): IV and 9 is 1 (I) less than 10 (X): IX. Only the following subtractive forms are used: 4 (IV), 9 (IX), 40 (XL), 90 (XC), 400 (CD) and 900 (CM).
Only powers of 10 (I, X, C, M) can be appended consecutively at most 3 times to represent multiples of 10. You cannot append 5 (V), 50 (L), or 500 (D) multiple times. If you need to append a symbol 4 times use the subtractive form.
Given an integer, convert it to a Roman numeral.

```
class Solution:
    def intToRoman(self, num: int) -> str:
        to_romans = {
            1 : "I",
            4: "IV",
            5 : "V",
            9: "IX",
            10 : "X",
            40 : "XL",
            50 : "L",
            90 : 'XC',
            100: "C",
            400: 'CD',
            500: "D",
            900: "CM",
            1000: "M"
        }
        
        res = ''
        cur = -1
        for x in sorted(to_romans, reverse=True):
            if num >= cur and cur != -1:                     
                res += num // cur * to_romans[cur]
                num = num % cur            
            cur = x
        res += num // cur * to_romans[cur]
        return res

```

# Experience

## Learning projects

* [G4U](https://se.cs.petrsu.ru/wiki/G4U)
* [P2P Systems](https://se.cs.petrsu.ru/wiki/P2P_Systems)

# Education
**Petrozavodsk State University**

Bachelor: *Applied mathematics and computer science*

# Languages

* **English** - B2 (Cambridge School)
* **Spanish** - A2
