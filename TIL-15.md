๐ฆTIL-15๐ฆ

# HTML์ Animation ์ ์ฉ ํ๋ ๋ฐฉ๋ฒ!
### 1. https://animate.style/ ์ ์
### 2. head ํ๊ทธ์ link ์ฐ๊ฒฐํ๊ธฐ
```html
<head>
  <link
    rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css"/>
</head>
```
### 3-1. ํด๋์ค ์ด๋ฆ์ผ๋ก ์ค์ ํ๊ธฐ
```html
<h1 class="animate__animated animate__bounce">An animated element</h1>
```
- `animate__animated animate__bounce`์ ๊ฐ์ด class๋ฅผ ์ ์ ํด์ผํ๋ค.
- ๋ง์ง๋ง์ `bounce` ๋ถ๋ถ์ ์ํ๋ animation์ผ๋ก ์ ์ฉํ๋ค. 

### 3-2. CSS๋ก ์ ์ฉํ๊ธฐ
```css
.my-element {
  display: inline-block;
  margin: 0 0.5rem;

  animation: bounce; /* ์ ๋๋ฉ์ด์ ์ข๋ฅ ์ค์  */
  animation-duration: 2s; /* ์ง์์๊ฐ ์ค์  */
  animation-delay: 1s; /* ์ง์ฐ์๊ฐ ์ค์  */
}
```
- ์ง์ฐ, ์ง์ ๊ธฐ๊ฐ์ ์ค์  ํ  ์ ์๋ค.
