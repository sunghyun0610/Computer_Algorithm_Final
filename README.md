๐ปComputer Algorithm final-term assingment๐ป
<br> by 201901671 ๋ฌธ์ฑํ
===========================================

## List
- **1.์ต์ ํด(์ ์ )์๊ณ ๋ฆฌ์ฆ ์๋ฆฌ ๋ฐ ์ค๋ช**
    - *1-1. P&Np(NP-hard)๋ฌธ์  ์๊ฐ*
    - *1-2. ์ฉ์ด ์ ๋ฆฌ(์ฌ์ ์ง์) ๋ฐ ์ ์ ์๊ณ ๋ฆฌ์ฆ ์๋ฆฌ ์ค๋ช*
- **2.์ ์ (Genetic) ์๊ณ ๋ฆฌ์ฆ์ผ๋ก ์ฝ๋(Python) ๋ฐ ๋์๋ฐฉ์ ์ค๋ช**
- **3.ํ๊ธฐ์**
- **4.๊ฐ์ ์ ๊ณผ ํ๋ฉด์ ์๋ก ๋ฐฐ์ฐ๊ณ  ๋๋ ์ **

## 1-1 **P&NP(NP-hard)๋ฌธ์  ์๊ฐ**
#### - Pย ๋ฌธ์ ๋ ๊ฒฐ์  ๋ฌธ์ ๋ค ์ค์์ย ์ฝ๊ฒ ํ๋ฆฌ๋ ๊ฒ์ ๋ชจ์ ๋์ ์งํฉ์ด๋ค. ์ด๋ค ๊ฒฐ์  ๋ฌธ์ ๊ฐ ์ฃผ์ด์ก์ ๋, ๋คํญ์(Polynomial) ์๊ฐ ์ด๋ด์ ๊ทธ ๋ฌธ์ ์ ๋ต์ YES์ NO ์ค์ ํ๋๋ก ๊ณ์ฐํด๋ผ ์ ์๋ ์๊ณ ๋ฆฌ์ฆ์ด ์กด์ฌํ๋ ๋ฌธ์ ์ด๋ค.     

#### -์์์๊ฐ์ ๋ค๋ฃจ์๋ **NP**(Non-deterministicย Polynomial)ย ๋ฌธ์ ๋ ํ์์ ์ผ๋ก๋, ๋ฌธ์ ๋ฅผ ํธ๋ ๊ฐ ๋จ๊ณ์์ ์ฌ๋ฌ๊ฐ์ง์ ๊ฐ๋ฅ์ฑ์ ๋์์ ๊ณ ๋ คํ  ์ ์๋ ๋น๊ฒฐ์ ์  ์๊ณ ๋ฆฌ์ฆ(non-deterministic algorithm)์ผ๋ก ๋คํญ์๊ฐ๋ด์ ๋ฌธ์ ๋ฅผ ํด๊ฒฐํ  ์ ์๋ ๋ฌธ์ ๋ผ๊ณ  ์ ์ํ๋ค. ์ฆ,์ด๋ค ๊ฒฐ์  ๋ฌธ์ ์ ๋ต์ด YES์ผ ๋, "๊ทธ ๋ฌธ์ ์ ๋ต์ด YES๋ผ๋ ๊ฒ์ ์์ฆํ๋ย ํํธ๊ฐ ์ฃผ์ด์ง๋ฉด, ๊ทธ ํํธ๋ฅผ ์ฌ์ฉํด์ ๊ทธ ๋ฌธ์ ์ ๋ต์ด ์ ๋ง๋ก YES๋ผ๋ ๊ฒ์ ๋คํญ์ ์๊ฐ ์ด๋ด์ ํ์ธํ  ์ ์๋ ๋ฌธ์ ๊ฐ ๋ฐ๋กย NPย ๋ฌธ์ ์ ํด๋น๋๋ค."</br>
![Alt text](https://upload.wikimedia.org/wikipedia/commons/4/4a/Complexity_classes.png)
#### ์ฌ์ค ๋ง์ ์ปดํจํฐ๊ณตํ์๋ค์ ์ ๋๋กย P=NP์ผ๋ฆฌ๊ฐ ์๋ค๊ณ  ๋ฏฟ๊ณ  ์๋ค. ์๋ํ๋ฉด,ย P=NP๊ฐ ์๋ฏธํ๋ ๋ฐ๋, ๋ง์ฝ ์ด๋ค ๋ฌธ์ ๊ฐ ์ฃผ์ด์ก์ ๋, ๊ทธ ๋ฌธ์ ์ ๋ต์์ ์ฝ๊ฒ ๊ฒ์ฐํ  ์ ์๋ค๋ฉด, ๊ทธ ๋ฌธ์  ์์ฒด๋ ์ฝ๊ฒ ํ ์ ์๋ค๋, ๋๋ฌด๋๋ ๊ฐ๋ ฅํ ์ฃผ์ฅ์ด๊ธฐ ๋๋ฌธ์ด๋ผ๊ณ  ์์์๊ฐ์ ๋ฐฐ์ ๋ค.</br>


## 1-2. **์ฉ์ด ์ ๋ฆฌ(์ฌ์ ์ง์) ๋ฐ ์ ์ ์๊ณ ๋ฆฌ์ฆ ์๋ฆฌ ์ค๋ช**
#### ์ ์  ์๊ณ ๋ฆฌ์ฆ์ ์๋ฌผ์ฒด๊ฐ ํ๊ฒฝ์ ์ ์ํ๋ฉด์ ์งํํด๊ฐ๋ ๋ชจ์ต์ ๋ชจ๋ฐฉํ์ฌ ~~์ต์ ํด~~๋ฅผ ์ฐพ์๋ด๋ ๊ฒ์ ๋ฐฉ๋ฒ์ด๋ค. ์ ์  ์๊ณ ๋ฆฌ์ฆ์ ์ด๋ก ์ ์ผ๋ก ์ ์ญ ์ต์ ์ ์ ์ฐพ์ ์ ์์ผ๋ฉฐ, ์ํ์ ์ผ๋ก ๋ชํํ๊ฒ ์ ์๋์ง ์์ ๋ฌธ์ ์๋ ์ ์ฉํ  ์ ์๊ธฐ ๋๋ฌธ์ ๋งค์ฐ ์ ์ฉํ๊ฒ ์ด์ฉ๋๋ค. ์ผ๋ฐ์ ์ผ๋ก ์ ์  ์๊ณ ๋ฆฌ์ฆ์ ๋ํด ์๊ณ ๋ฆฌ์ฆ์ด๋ผ๋ ํํ์ ์ด์ฉํ์ง๋ง, ์ ์  ์๊ณ ๋ฆฌ์ฆ์ ํน์ ํ ๋ฌธ์ ๋ฅผ ํ๊ธฐ ์ํ ์๊ณ ๋ฆฌ์ฆ์ด๋ผ๊ธฐ ๋ณด๋ค๋ **์ต์ ํ ๋ฌธ์ ๋ฅผ ํ๊ธฐ ์ํ ๋ฐฉ๋ฒ๋ก **์ ๊ฐ๊น๋ค. ์ฆ, ๋ชจ๋  ๋ฌธ์ ์ ์ ์ฉ ๊ฐ๋ฅํ ํ๋์ ์๊ณ ๋ฆฌ์ฆ์ด๋ ์์ค ์ฝ๋๊ฐ ์๋ ๊ฒ์ด ์๋๊ธฐ ๋๋ฌธ์ ์ ์  ์๊ณ ๋ฆฌ์ฆ์ ์๋ฆฌ๋ฅผ ์ดํดํ๊ณ , ์ด๋ฅผ ์์ ์ด ์ํ๋ ๋ฌธ์ ์ ์ ์ฉํ  ์ ์๋๋ก ํ๋ ๊ฒ์ด ์ค์ํ๋ค๊ณ  ์๊ฐํ๋ค.
### ์ฉ์ด์ ๋ฆฌ
- **์ผ์์ฒด(chromosome)**: ์ ์  ์๊ณ ๋ฆฌ์ฆ์์ ํ๋์ ํด (solution)๋ฅผ ํํํ๋ค. ์ฆ ์ด๋ ํ ๋ฌธ์ ์ ํด๋ฅผ ์ผ์์ฒด๋ก ์นํํ ๊ฒ์ด๋ค.
- **์ ์ ์(gene)**: ์ผ์์ฒด๋ฅผ ๊ตฌ์ฑํ๋ ์์. ํ๋์ ์ ์  ์ ๋ณด๋ฅผ ๋ํ๋ธ๋ค. ์ด๋ ํ ์ผ์์ฒด์ ์ ์ ์๊ฐ [A B C]๋ผ๋ฉด, ์ด ์ผ์์ฒด์๋ ๊ฐ๊ฐ A, B, C์ ๊ฐ์ ๊ฐ๋ 3๊ฐ์ gene์ด ์กด์ฌํ๋ค.
- **์์ (offspring)**: ํน์  ์๊ฐ t์ ์กด์ฌํ๋ ์ผ์์ฒด๋ค๋ก๋ถํฐ ์์ฑ๋ ์ผ์์ฒด๋ฅผ t์ ์กด์ฌํ๋ ์ผ์์ฒด๋ค์ ์์์ด๋ผ๊ณ  ํ๋ค. ์์์ ์ด์  ์ธ๋์ ๋น์ทํ ์ ์  ์ ๋ณด๋ฅผ ๊ฐ๋๋ค.
- **์ ํฉ๋ (fitness)**: ํด๋น ๋ฌธ์ ์ ๋ํด ์ผ์์ฒด๊ฐ ํํํ๋ ํด๊ฐ ์ผ๋ง๋ ์ ํฉํ์ง๋ฅผ ๋ํ๋ธ๋ค.
์ ์ ํ์ ์ผ๋ก๋ ์ผ์์ฒด๊ฐ ๊ฐ๊ณ  ์๋ ๊ณ ์ ๊ฐ์ ๋ปํ๋ค.

### ์๊ณ ๋ฆฌ์ฆ ๊ตฌ์กฐ
1. #### ์ด๊ธฐ ์ผ์๊ฒ์ ์งํฉ ์์ฑ
2. #### ์ด๊ธฐ ์ผ์์ฒด๋ค์ ๋ํ ์ ํฉ๋ ๊ณ์ฐ
3. #### ํ์ฌ ์ผ์์ฒด๋ค๋ก๋ถํฐ ์์๋ค์ ์์ฑ
4. #### ์์ฑ๋ ์์๋ค์ ์ ํฉ๋ ๊ณ์ฐ
5. #### ์ข๋ฃ ์กฐ๊ฑด ํ๋ณ
6. #### ์ข๋ฃ ์กฐ๊ฑด ๊ฑฐ์ง์ด๋ฉด->3์ผ๋ก ์ด๋ํ์ฌ ๋ฐ๋ณต
#### =>์ฆ ์ผ์์ฒด์งํฉ์์ ์ ํฉ๋๊ฐ ๊ฐ์ฅ ์ข์ ์ผ์์ฒด๋ฅผ ์ ํํ๊ณ , ์ ํ๋ ํด์ ๋ฐฉํฅ์ผ๋ก ๊ฒ์น์ ๋ฐ๋ณตํ๋ฉด์ "์ต์ ํด"๋ฅผ ์ฐพ์๊ฐ๋ ๊ตฌ์กฐ์ด๋ค.

### ์ฐ์ฐ ์ ์
#### ์ ์ ์๊ณ ๋ฆฌ์ฆ์ ์์ ์ธ๊ธํ๋ ๊ฒ์ฒ๋ผ ์์ ์ด ์ํ๋ ๋ฌธ์ ์ ์ ์ฉํ  ์ ์๋ค.์ด๋ฅผ ์ํด์  ์ด 5๊ฐ์ ์ฐ์ฐ์ ์ ์ํ๊ณ  ์ดํดํด์ผํ๋ค.
#### 1. ์ด๊ธฐ ์ผ์์ฒด ์์ฑ ์ฐ์ฐ.
#### ->์ด๊ธฐ์๋ ์ด์  ์ผ์์ฒด๊ฐ ์กด์ฌํ์ง ์๊ธฐ ๋๋ฌธ์ ์ ํ๋ ์ผ์์ฒด๋ค๋ก๋ถํฐ ์์์ ์์ฑํ  ์๊ฐ ์๋ค. ๋ฐ๋ผ์, ์ด๊ธฐ ์ผ์์ฒด๋ฅผ ์์ฑํ๋ ์ฐ์ฐ์ ๋ณ๋๋ก ์ ์ํด์ผ ํ๋ค. 
```
Random rand = new Random();
int[] chromosome = new int[SIZE_CHROMOSOME];
 
for(int i = 0; i < SIZE_CHROMOSOME; i++) {
    chromosome[i] = rand.nextInt(MAX_VAL_GENE);
}
```
#### ์ด์ ๊ฐ์ ๋ฐฉ๋ฒ์ ์ด๋ ํ ๊ท์น๋ ์์ด ์์์ ๊ฐ์ผ๋ก ์ผ์์ฒด๋ฅผ ์์ฑํ๋ ๊ฒ์ผ๋ก ์ด๋ฏธ ๋ฐ์ดํฐ๊ฐ์๋ ๊ฒฝ์ฐ์๋ ๋ฐฐ์ด์ ์ง์  ์๋ ฅํ๋ฉด ๋ ๊ฒ์ด๋ค.

#### 2. ์ ํฉ๋๋ฅผ ๊ณ์ฐํ๋ ์ฐ์ฐ
#### -> ์ผ์์ฒด์ ํํ๋ ์ ๋ณด๋ฅผ ๊ธฐ๋ฐ์ผ๋ก ์ ํฉ๋๋ฅผ ๊ณ์ฐํ๋ ์ฐ์ฐ 

#### 3. ์ ํฉ๋๋ฅผ ๊ธฐ์ค์ผ๋ก ์ผ์์ฒด ์ ํํ๋ ์ฐ์ฐ
#### ->๋จ์ํ ์ ํฉ๋๊ฐ ๊ฐ์ฅ ๋์ ๋๊ฐ๋ฅผ ์ ํํ๋ ๊ฒ์ ๋ค์์ฑ์์ด ํฌ๊ฒ ์ ํ๋๊ธฐ๋๋ฌธ์ ์ต์ ํด๋ฅผ ์ฐพ๊ธฐ์๋ ๋ถ์กฑํ  ๊ฒ์ด๋ค. ์ด๋ฅผ ๋ณด์ํ๊ธฐ ์ํด์ "๋ฃฐ๋  ํ  ์ ํ" ๋ฐฉ๋ฒ์ ์ฌ์ฉํ๋ค.
#### P(ch.j)=f(Ch.j)/โ(i๋ถํฐN๊น์ง)f(Ch.i)์ ๊ฐ์ ์์
![Alt text](https://t1.daumcdn.net/cfile/tistory/260E9E3957DBBC7C15?download)
#### ์ฆ ์์ ์์์ ์ด์ฉํ์ฌ ๋ฃฐ๋ ์ ๋ง๋ค๊ณ  ์ด๋ฅผ ์ด์ฉํ์ฌ ํ๋ฅ ์ ์ผ๋ก ์ผ์์ฒด๋ฅผ ์ ํํ๋ ๊ฒ์ด๋ค.


#### 4.  ์ ํ๋ ์ผ์์ฒด๋ค๋ก๋ถํฐ ์์์ ์์ฑํ๋ ์ฐ์ฐ
#### ์ ํ๋ ๋๊ฐ์ ๋ถ๋ชจ ์ผ์์ฒด๋ค๋ก ๋ถํฐ ์ด์  ์์ ์ผ์์ฒด๋ฅผ ์์ ํ๋ ๋จ๊ณ์ด๋ค. ์ฐ๋ฆฌ๊ฐ ์ ์๊ณ ์๋ ๊ฒ์ฒ๋ผ ๋ถ ์ ์ ์ + ๋ชจ ์ ์ ์๊ฐ ์กฐํฉ๋์ด =์์์ ์ ์๊ฐ ๋๋ค. ์ด๋ ๋ฏ ์ผ์์ฒด๋ฅผ ๋ถํ ํ๋ ํ์๋ฅผ "Crossover"๋ผ ํ๊ณ  ๋ถ ์ ์ ์์ ๋ชจ์ ์ ์๋ฅผ ๋ถํ ํ๋ ์ง์ ์ธ division point๋ ์์๋ก ์ ํ๋๋ค.
#### 5. ***๋์ฐ๋ณ์ด*** ์ฐ์ฐ
#### ๋๋์ด ์ ์ ์๊ณ ๋ฆฌ์ฆ์ ํต์ฌ์ด๋ผ๊ณ  ํ  ์ ์๋ "๋์ฐ๋ณ์ด"๋ฅผ ๊ณ์ฐํ  ์ฐจ๋ก์ด๋ค. ๋์ฐ๋ณ์ด ์์๋ฅผ ์ถ๊ฐํ๋ ์ด์ ๋ ์ ์  ์๊ณ ๋ฆฌ์ฆ์์๋ ์ง์ญ ์ต์ ์ ์ ๋น ์ง๋ ๋ฌธ์ ๋ฅผ ํด๊ฒฐํ๊ธฐ ์ํด ์๋กญ๊ฒ ์์ฑ๋ ์ผ์์ฒด์ ํ๋ฅ ์ ์ผ๋ก ๋์ฐ๋ณ์ด๊ฐ ๋ฐ์ํ๋๋ก ํ๋ ๊ฒ์ด๋ค.(์ผ๋ฐ์ ์ผ๋ก 0.05%์์ค์ ๋ฎ์ ํ๋ฅ )
![Alt text](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=http%3A%2F%2Fcfile24.uf.tistory.com%2Fimage%2F236D374857DBC2AF2C3A50)
#### <br> ๋์ฐ๋ณ์ด๋ ๋๊ฐ์ง ์ข๋ฅ๊ฐ ์๋๋ฐ
- a)reverse: ํ๋์ ์ ์ ์๊ฐ 0->1 ๋๋ 1->0 ์ผ๋ก ๋ค์ง์ด์ง๋ ๋์ฐ๋ณ์ด
- b)exchange: ์์์ ๋๊ฐ์ ์ ์ ์๊ฐ ์๋ก ๊ตํ๋๋ ๋์ฐ๋ณ์ด

## **2.์ ์ (Genetic) ์๊ณ ๋ฆฌ์ฆ์ ์ด์ฉํ TSP ์ฝ๋(Python) ๋ฐ ๋์๋ฐฉ์ ์ค๋ช**
#### ์ ์  ์๊ณ ๋ฆฌ์ฆ์ ์ด์ฉํ ๋ํ์ ์ธ ๋ฌธ์ ์ธ TSP์๋ํ ๊ตฌํ ์ฝ๋ ๋ฐ ์ค๋ช์ #(์ฃผ์)์ํตํด ์ค๋ชํด๋ณด์๋ค.
#### ์ ์ ์ฃผ์ ๋ ์คํํ์ปค๋ฆฌ์ ๊ณจ๋์์ ๊ฑฐ๋ฆฌ์ ๋ฐ๋ฅธ ์์ฑ๊ณต๋ฅ  ๋ณํ ์ด์ง๋ง ์ฝ๋์ ์ ์ฉํด ๋ณด๋ ๊ฒ์ ํ๊ณ๊ฐ ์์ด์ ์ฝ๋ ์ค๋ช์ TSP๋ก ํ์์ต๋๋ค!
#### ์ฝ๋๋ ๊นํ๋ธ ๋ ํฌ์งํ ๋ฆฌ์๋ ์์ง๋ง readmeํ์ผ์๋ ์ฒจ๋ถํ๊ฒ ๋ค.

```

import math
import random
import cv2#map์ด์ฉํ๋ ํจํค์ง


class City:# ํ ๋์์๋ฏธ
   def __init__(self, x=None, y=None):
      self.x = None#๋์์ x์ขํ ์ง์ 
      self.y = None#๋์์ y์ขํ ์ง์ 
      if x is not None:
         self.x = x
      else:
         self.x = int(random.random() * 200)
      if y is not None:
         self.y = y
      else:
         self.y = int(random.random() * 200)
   
   def getX(self):
      return self.x
   
   def getY(self):
      return self.y
   
   def distanceTo(self, city):#๋ค๋ฅธ ๋์๊ฐ์ ๊ฑฐ๋ฆฌ ๊ฐ
      xDistance = abs(self.getX() - city.getX())
      yDistance = abs(self.getY() - city.getY())
      distance = math.sqrt( (xDistance*xDistance) + (yDistance*yDistance) )
      return distance
   
   def __repr__(self):
      return str(self.getX()) + ", " + str(self.getY())


class TourManager:#๊ฐ ๋์๋ค์ ์ฐ๊ฒฐํ ๊ฒฝ๋ก
   destinationCities = []
   
   def addCity(self, city):
      self.destinationCities.append(city)
   
   def getCity(self, index):
      return self.destinationCities[index]
   
   def numberOfCities(self):
      return len(self.destinationCities)


class Tour:
   def __init__(self, tourmanager, tour=None):
      self.tourmanager = tourmanager
      self.tour = []
      self.fitness = 0.0#fitness=์ ์ , ๊ฑฐ๋ฆฌ์ ๋ฐ๋น๋ก
      self.distance = 0
      if tour is not None:
         self.tour = tour
      else:
         for i in range(0, self.tourmanager.numberOfCities()):
            self.tour.append(None)
   
   def __len__(self):
      return len(self.tour)
   
   def __getitem__(self, index):
      return self.tour[index]
   
   def __setitem__(self, key, value):
      self.tour[key] = value
   
   def __repr__(self):
      geneString = "|"
      for i in range(0, self.tourSize()):
         geneString += str(self.getCity(i)) + "|"
      return geneString
   
   def generateIndividual(self):
      for cityIndex in range(0, self.tourmanager.numberOfCities()):
         self.setCity(cityIndex, self.tourmanager.getCity(cityIndex))
      random.shuffle(self.tour)
   
   def getCity(self, tourPosition):
      return self.tour[tourPosition]
   
   def setCity(self, tourPosition, city):
      self.tour[tourPosition] = city
      self.fitness = 0.0
      self.distance = 0
   
   def getFitness(self):
      if self.fitness == 0:
         self.fitness = 1/float(self.getDistance())# ๊ฑฐ๋ฆฌ๊ฐ ์งง์์๋ก ์ ์๊ฐ ๋๋ค!
      return self.fitness
   
   def getDistance(self):#tour์ ์ด๊ฑฐ๋ฆฌ๋ฅผ ๊ณ์ฐํ๋ ํจ์
      if self.distance == 0:
         tourDistance = 0
         for cityIndex in range(0, self.tourSize()):
            fromCity = self.getCity(cityIndex)
            destinationCity = None
            if cityIndex+1 < self.tourSize():
               destinationCity = self.getCity(cityIndex+1)
            else:
               destinationCity = self.getCity(0)
            tourDistance += fromCity.distanceTo(destinationCity)
         self.distance = tourDistance
      return self.distance
   
   def tourSize(self):
      return len(self.tour)
   
   def containsCity(self, city):
      return city in self.tour

#์ ์  ์๊ณ ๋ฆฌ์ฆ ์์!
class Population:#tour๋ค์ ๋ชจ์, 50๊ฐ์ popultaion์์ฑํ๋ค=50๊ฐ์ ํฌ์ด๊ฐ ์๋ค. ์ฌ๋ฌ๊ฐ์ง ํฌ์ด ๊ฑฐ๋ฆฌ๋ค์ ๊ณ์ฐํ๊ณ  fitness(์ ์)๊ฐ ๋์๊ฒ๋ค์ mutate(๋์ฐ๋ณ์ด)+crossoverํด์ ์ต์ ํด ์ฐพ๋ ๊ณผ์ 
   def __init__(self, tourmanager, populationSize, initialise):
      self.tours = []
      for i in range(0, populationSize):
         self.tours.append(None)
      
      if initialise:
         for i in range(0, populationSize):
            newTour = Tour(tourmanager)
            newTour.generateIndividual()
            self.saveTour(i, newTour)
      
   def __setitem__(self, key, value):
      self.tours[key] = value
   
   def __getitem__(self, index):
      return self.tours[index]
   
   def saveTour(self, index, tour):
      self.tours[index] = tour
   
   def getTour(self, index):
      return self.tours[index]
   
   def getFittest(self):
      fittest = self.tours[0]
      for i in range(0, self.populationSize()):
         if fittest.getFitness() <= self.getTour(i).getFitness():
            fittest = self.getTour(i)
      return fittest
   
   def populationSize(self):
      return len(self.tours)


class GA:#์ ์  ์๊ณ ๋ฆฌ์ฆ์ ํต์ฌ
   def __init__(self, tourmanager):
      self.tourmanager = tourmanager
      self.mutationRate = 0.015#๋์ฐ๋ณ์ด ์ผ์ด๋  ํ๋ฅ 
      self.tournamentSize = 5
      self.elitism = True
   
   def evolvePopulation(self, pop):#์งํ๊ณผ์ 
      newPopulation = Population(self.tourmanager, pop.populationSize(), False)
      elitismOffset = 0
      if self.elitism:
         newPopulation.saveTour(0, pop.getFittest())
         elitismOffset = 1
      
      for i in range(elitismOffset, newPopulation.populationSize()):
         parent1 = self.tournamentSelection(pop)
         parent2 = self.tournamentSelection(pop)
         child = self.crossover(parent1, parent2)
         newPopulation.saveTour(i, child)
      
      for i in range(elitismOffset, newPopulation.populationSize()):
         self.mutate(newPopulation.getTour(i))
      
      return newPopulation
   
   def crossover(self, parent1, parent2):#crossover
      child = Tour(self.tourmanager)
      
      startPos = int(random.random() * parent1.tourSize())
      endPos = int(random.random() * parent1.tourSize())
      
      for i in range(0, child.tourSize()):
         if startPos < endPos and i > startPos and i < endPos:
            child.setCity(i, parent1.getCity(i))
         elif startPos > endPos:
            if not (i < startPos and i > endPos):
               child.setCity(i, parent1.getCity(i))
      
      for i in range(0, parent2.tourSize()):
         if not child.containsCity(parent2.getCity(i)):
            for ii in range(0, child.tourSize()):
               if child.getCity(ii) == None:
                  child.setCity(ii, parent2.getCity(i))
                  break
      
      return child
   
   def mutate(self, tour):#๋ณ์ด๊ณผ์ 
      for tourPos1 in range(0, tour.tourSize()):
         if random.random() < self.mutationRate:
            tourPos2 = int(tour.tourSize() * random.random())
            
            city1 = tour.getCity(tourPos1)
            city2 = tour.getCity(tourPos2)
            
            tour.setCity(tourPos2, city1)
            tour.setCity(tourPos1, city2)
   
   def tournamentSelection(self, pop):
      tournament = Population(self.tourmanager, self.tournamentSize, False)
      for i in range(0, self.tournamentSize):
         randomId = int(random.random() * pop.populationSize())
         tournament.saveTour(i, pop.getTour(randomId))
      fittest = tournament.getFittest()
      return fittest



if __name__ == '__main__':
    n_cities = 20
    population_size = 50
    n_generations = 100

    random.seed(100)

    # Load the map
    map_original = cv2.imread('map.jpg')

    # Setup cities and tour
    tourmanager = TourManager()

    for i in range(n_cities):
        x = random.randint(200, 800)
        y = random.randint(200, 800)

        tourmanager.addCity(City(x=x, y=y))
        cv2.circle(map_original, center=(x, y), radius=10, color=(0, 0, 255), thickness=-1, lineType=cv2.LINE_AA)

    cv2.imshow('map', map_original)
    cv2.waitKey(0)

    # Initialize population
    pop = Population(tourmanager, populationSize=population_size, initialise=True)
    print("Initial distance: " + str(pop.getFittest().getDistance()))

    # Evolve population
    ga = GA(tourmanager)

    for i in range(n_generations):
        pop = ga.evolvePopulation(pop)

        fittest = pop.getFittest()

        map_result = map_original.copy()

        for j in range(1, n_cities):
            cv2.line(
                map_result,
                pt1=(fittest[j-1].x, fittest[j-1].y),
                pt2=(fittest[j].x, fittest[j].y),
                color=(255, 0, 0),
                thickness=3,
                lineType=cv2.LINE_AA
            )

        cv2.putText(map_result, org=(10, 25), text='Generation: %d' % (i+1), fontFace=cv2.FONT_HERSHEY_SIMPLEX, fontScale=0.7, color=0, thickness=1, lineType=cv2.LINE_AA)
        cv2.putText(map_result, org=(10, 50), text='Distance: %.2fkm' % fittest.getDistance(), fontFace=cv2.FONT_HERSHEY_SIMPLEX, fontScale=0.7, color=0, thickness=1, lineType=cv2.LINE_AA)
        cv2.imshow('map', map_result)
        if cv2.waitKey(100) == ord('q'):
            break

    # Print final results
    print("Finished")
    print("Final distance: " + str(pop.getFittest().getDistance()))
    print("Solution:")
    print(pop.getFittest())

    cv2.waitKey(0)
```
#### ์ ์  ์๊ณ ๋ฆฌ์ฆ์์ ๋์ฐ๋ณ์ด๋ ์ง์ญ ์ต์ ์ ์ ๋น ์ง๋ ๋ฌธ์ ๋ฅผ ํด๊ฒฐํ๊ธฐ ์ํด ์๋กญ๊ฒ ์์ฑ๋ ์ผ์์ฒด์ ํ๋ฅ ์ ์ผ๋ก ๋์ฐ๋ณ์ด๊ฐ ๋ฐ์ํ๋๋ก ํ๋ ๊ฒ์ด๋ค.(์ผ๋ฐ์ ์ผ๋ก 0.05%์์ค์ ๋ฎ์ ํ๋ฅ )
- ๋์ฐ๋ณ์ด ํ๋ฅ ์ด ๋๋ฌด ๋์ ๊ฒฝ์ฐ: ๋๋ฌด ๋ง์ ๋ณ์ด๊ฐ ๋ฐ์ํด ์๊ฐ๋ณต์ก๋๊ฐ ์ฆ๊ฐํ๋ค
- ๋์ฐ๋ณ์ด ํ๋ฅ ์ด ๋๋ฌด ๋ฎ์ ๊ฒฝ์ฐ: ๋ชจ๋  ๊ฒฝ์ฐ์ ์๋ฅผ ๋ค ๊ณ ๋ คํ์ง ๋ชปํ์ฌ ์ต์ ํด๋ฅผ ๊ตฌํ  ํ๋ฅ ์ด ๋ฎ์์ง๋ค. 
#### ๋ผ๊ณ   ์ ๋ฆฌํ  ์ ์๊ฒ ์ต๋๋ค.
#### ์ฌ๊ธฐ๊น์ง ์ ์ ์๊ณ ๋ฆฌ์ฆ์ ๋ํด ์์๋ณด์๊ณ  ์ด์  ์ ๊ฐ ์ ํ ์ฃผ์ ๋ฅผ ์๊ฐํ๊ฒ ์ต๋๋ค.
## **3.ํ๊ธฐ์**
# Topic : ํด๋ฆญํ์์ ๋ฐ๋ฅธ ๊ด๊ณ  ๋ธ์ถ ๋น๋ ๋ฐ์ดํฐ ๊ทธ๋ํ์ ํ๊ธฐ์
/*ํ๊ท์์ด๋? Y=f(x)์์ ํ์ชฝ์ ๋ณ์์์ ๋ค๋ฅธ์ชฝ์ ๋ณ์ ๊ฐ์ ์์ธกํ๊ธฐ ์ํ ๋ฐฉ์ ์์ ํ๊ท์์ด๋ผ ํ๊ณ  Y๋ฅผ ์ข์๋ณ์, X๋ฅผ ๋๋ฆฝ ๋ณ์๋ผ๊ณ  ํ๋ค.*/
![Alt text](https://github.com/sunghyun0610/Computer_Algorithm_Final/blob/main/%ED%9A%8C%EA%B7%80%EC%8B%9D%20%EA%B7%B8%EB%9E%98%ED%94%84%20%EC%98%88.png?raw=true)
#### ํด๋ฆญํ์์ ๋ฐ๋ฅธ ๊ด๊ณ  ๋ธ์ถ ๋น๋ ๋ฐ์ดํฐ ๊ทธ๋ํ์ ํ๊ธฐ์
![Alt text](https://github.com/sunghyun0610/Computer_Algorithm_Final/blob/main/%EA%B4%91%EA%B3%A0-%ED%81%B4%EB%A6%AD%20%EB%8D%B0%EC%9D%B4%ED%84%B0.png?raw=true)
![Alt text](https://github.com/sunghyun0610/Computer_Algorithm_Final/blob/main/%ED%9A%8C%EA%B7%80%EC%8B%9D.png?raw=true)
#### ์ถ๊ฐ๋ก ๋ด๊ฐ ๊ด์ฌ์๋ ์ฃผ์ ๋ ํด๋ณด์๋ค.
### Topic2 : ๊ฑฐ๋ฆฌ์ ๋ฐ๋ฅธ ์คํํ ์ปค๋ฆฌ์ ์ ์ฑ๊ณต๋ฅ  ๋ณํ๋ฅผ ๋งค๋ฌ ์ฃผ๊ธฐ๋ก ์์๋ณด๊ณ  ํ๊ธฐ์์ ํตํด ์ค์ฐจ๋ฅผ ์ต์ํ๋๊ฒ ๋ค์๋ฌ ์์ธก.
![Alt text](https://github.com/sunghyun0610/Computer_Algorithm_Final/blob/main/%EC%8A%A4%ED%85%8C%ED%94%88%20%EC%BB%A4%EB%A6%AC%20%ED%9A%8C%EA%B7%80%EC%8B%9D!!.png?raw=true)
#### ๋์ค์ ๊ธฐํ๊ฐ ๋๋ค๋ฉด ์ด ์ฃผ์ ๋ ์ ์ ์๊ณ ๋ฆฌ์ฆ์ผ๋ก ์ต์ ํด๋ฅผ ๊ตฌํ  ์ ์๋์ง ์์๋ณด๊ฒ ๋ค.
## **4.๊ฐ์ ์ ๊ณผ ํ๋ฉด์ ์๋ก ๋ฐฐ์ฐ๊ณ  ๋๋ ์ **
#### ์ฐ์  ์ด๋ฒํ๊ธฐ ๊ฐ์ฅ ๊ธฐ์ต์ ๋จ๋ ์์์ด ๋ญ๋ ํ๋ฉด ๋น์ฐ ์ปดํจํฐ ์๊ณ ๋ฆฌ์ฆ ์์์์ต๋๋ค. ๋จ์ ์ฝ๋ฉ ๋ฐ์ ๋ชฐ๋๋ ์ ๋ฅผ ์๊ณ ๋ฆฌ์ฆ ๋ฐ github์ฌ์ฉ๋ฒ์ ์กฐ๊ธ์ด๋๋ง ๊นจ๋ซ๊ฒ ํด์ฃผ์  ๊น๋ํ ๊ต์๋ ๊ฐ์ฌํฉ๋๋ค. ์ํํธ์จ์ด ๊ฐ๋ฐ์๊ฐ ๋๊ธฐ์ํด ์๊ณ ๋ฆฌ์ฆ์ ์ค์์ฑ์ ๋ค์ํ๋ฒ ๋๊ผ๊ณ  ์์ผ๋ก ๊ณต๋ถ ๋ฐฉํฅ์ฑ์ ์ก์ ์ ์์ ๊ฒ๊ฐ์ต๋๋ค.
#### ๋ ์ด๋ฒ ์ ์  ์๊ณ ๋ฆฌ์ฆ ๋ฐ ์ต์ ํด ์๊ณ ๋ฆฌ์ฆ์ ๊ณต๋ถํ๋ฉด์ ํ๋ก๊ทธ๋๋ฐ์ผ๋ก ์ ๋ง ๋ค์ํ ๊ฑธ ๋ง๋ค ์ ์๊ตฌ๋ ๋๊ผ์ต๋๋ค. ์ด์ ๋ฐ๋ฉด ์์ง ์ ์ ์ค๋ ฅ์ ๋ง์ด ๋ถ์กฑํ ๊ฒ๊ฐ๊ณ  ์์ง 2ํ๋์ด๋๊น ๋ ์ด์ฌํ ํ  ๋๊ธฐ๊ฐ ๋๊ฒ ๊ฐ์ต๋๋ค. ๊ฐ์ฌํฉ๋๋ค ๋ฐฉํ ์ ๋ณด๋ด์ญ์ผ!