๐ฒTIL-14๐ฒ

# position
: ์์น์ ๊ธฐ์ค์ ์ง์ ํ๋ค.
- ๊ธฐ์ค์ ์ง์ ํ ๋ค์ top,bottom,left,right๋ก ์์น๋ฅผ ์ง์ ํ๋ค.

## position : relative
: ์๋ __์๊ธฐ ์์ __์ด ์์๋ ์์น๋ฅผ ๊ธฐ์ค์ผ๋ก ์ก๋๋ค.

## position : absolute
: ๋ณด๋ชจ ์์ ์ค __๊ฐ์ฅ ์ต๊ทผ์ position__์ ๊ฐ์ง๋ ์์น๋ฅผ ๊ธฐ์ค์ผ๋ก ์ก๋๋ค.
- ์์ ์์์์ absolute๋ฅผ ์ฐ๊ธฐ์ํด์  ๋ถ๋ชจ ์์์ relative๋ฅผ ๋ถ์ฌํด์ผ ํ๋ค.

## position : fixed
: view port(ํ๋ฉด ์์ฒด)๋ฅผ ๊ธฐ์ค์ผ๋ก ์์น๋ฅผ ์ก๋๋ค.
ex) ์ผํ๋ชฐ์ ๊ด๊ณ  ๋ฒ ๋ ๋ฑ๋ฑ..

## position : sticky
: ์คํฌ๋กค์ ์๋จ์ ๋ถ์ด์ ์์ง์, JS๋ฅผ ์ฐ์ง ์๊ณ  ์ฝ๊ฒ ๊ตฌํ ๊ฐ๋ฅํ๋ค.

# background
: ๋ฐฐ๊ฒฝ์ ์ง์ ํ๋ค. ์ด๋ฏธ์ง, ์์์ ์ฃผ๋ก ์ฌ์ฉ๋๋ค.
- `background-img: url();`: ์ด๋ฏธ์ง๋ฅผ ์ง์ ํ  ์ ์๋ค,
- `background-size: (width) (height)` : ์ด๋ฏธ์ง์ ์ฌ์ด์ฆ๋ฅผ ์ง์ ํ  ์ ์๋ค.
    - __`background-size: (width)` ๋ง ์ฌ์ฉํ์ฌ ์ด๋ฏธ์ง๋ฅผ ์ฐ๊ทธ๋ฌํธ๋ฆฌ์ง ์๊ณ  ์ฌ์ฉํ์!!__
- `background-repeat:no-repeat`: ๋ฐ๋ณต์ ๋ฉ์ถ๋ค.
    - background์ ์ง์  ํฌ๊ธฐ์์ ์ด๋ฏธ์ง ์ฌ์ด์ฆ๋ฅผ ์ง์ ํ๋ฉด ๋จ๋ ํฌ๊ธฐ๋งํผ ๋ฐ๋ณต๋๋ค.  

# transition
: ๋ฐ๋๊ธฐ ์ ์ ํ๊ทธ์ ์์ฑ์ ๋ถ์ฌํ๋ฉฐ ๋ฐ๋ ๊ฒ(property)๊ณผ ์๊ฐ(duration)์ ์ง์ ํ๋ค.
```css
.box{
  width: 100px;
  height: 100px
  background:tomato;
  transition : width 1s;   // 1์ด๋์ width๋ฅผ ๋ฐ๊พผ๋ค
}
.box:hover{
  width: 200px;
}
```
- `transition : width 1s` = `transition-property :width; ,  transition-during:1s` 
- __๊ฐ์ ์ ํ์์ ์ง์ผ๋ก ์ฌ์ฉ์ ์ ๋๋ฉ์ด์ ๊ธฐ๋ฅ์ผ๋ก ์ฌ์ฉ ๊ฐ๋ฅ!!!!!__

# ์ด๋ (transform)
```css
.box{
  width: 100px;
  height: 100px
  background:tomato;
  transition: 1s;  // 1์ด๋์
  
.box:hover{
  transform: translate(30px,30px)    // ๋ง์ฐ์ค ์ฌ๋ฆฌ๋ฉด ํด๋น ์์น๋ก ์ด๋ํจ
}
```

# ํฌ๊ธฐ (transform)
```css
.box{
  width: 100px;
  height: 100px
  background:tomato;
  transition: 1s;  // 1์ด๋์
  
.box:hover{
  transform: scale(2)    // ๋ง์ฐ์ค ์ฌ๋ฆฌ๋ฉด 2๋ฐฐ๋ก ๋์ด๋จ 
  }
```
     
