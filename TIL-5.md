๐ณTIL-5๐ณ

## ๐ฆ์ฌ๋ฌ๊ฐ์ง ์์ฑ
```css
.box{
    width: 100px;
    height: 70px;
    background: red;
    font-size: 16px;
    margin: 20px;
    padding: 20px;
}
```
- .box๋ ํด๋์ค ์ด๋ฆ์ผ๋ก ์ฐพ๋ ๋ฐฉ๋ฒ์!
- ๋จ์๋ px
- ๊ทธ๋ฅcolor ์์ฑ์ด ํ์คํธ ์๊น์!! (HTML์ content ๋ถ๋ถ)

## ๐ฆ์ฝ๋ ํ์ธ ๋ฐฉ๋ฒ

![image](https://user-images.githubusercontent.com/67450413/117403217-cb649100-af42-11eb-9210-d7ac829e38b4.png)

- ์ด์ ๊ฐ์ด live server๋ฅผ ์ด์ฉํ ํ ์น์์ `F12` ๊ฐ๋ฐ์ ๋ชจ๋ ๋๋ฅด๋ฉด ํ์ธ ๊ฐ๋ฅ!
- ๋ด๊ฐ ํ์์ ๋ณด๊ณ  ๊ด์ฐฎ๋ค๊ณ  ์๊ฐํ ๋์์ธ์ด๋ ์์ ์กฐํฉ ํ์ธ ๊ฐ๋ฅํ๋ค๋๊ฒ ์ต๋ ์ฅ์ !

## ๐ฆํน์ดํ ์์ฑ
### 1. ์ํ
```css
.clearfix::after{
    content: "";
    display: block;
    clear: both;
}    
```
์๋ฅผ ํ๊ณ  `1. HTML ํด๋์ค์ clearfix ์ถ๊ฐ` , `2. css ์ ํ์ ์์ float: left;` ํ๋ฉด ์ํ์ผ๋ก ๋ณด์ด๊ฒ ๋ง๋ค ์ ์์

### 2. ์ค์ 
`border-bottom: 1px solid lightgray;`

### 3. ํน์ดํ๊ฒ ์ ํ์ ์ ํํ๋ ๋ฒ
```css
.logo img {
    display: block;
}
```
-> .logo ํด๋์ค ์์ ์๋ img ํ๊ทธ๋ง ์ง์ ํด ์ค!
