π»TIL-10π»

# form νκ·Έ
: μΉ μλ²μ μ λ³΄λ₯Ό μ μΆνκΈ° μν μμ λ²μλ₯Ό μ μνλ€.

![image](https://user-images.githubusercontent.com/67450413/120430755-75083800-c3b2-11eb-8e58-ad001f3342ee.png)
- action: μ μ‘ λ°μ URL
- method="GET" -> urlμ μλ ₯κ° λνλ
- method="POST" -> urlμ μλ ₯κ° λνλ΄μ§ μμ


# Input νκ·Έ
: μ¬μ©μμκ² μλ ₯ λ°μ λ°μ΄ν° μμ

![image](https://user-images.githubusercontent.com/67450413/120432255-a08c2200-c3b4-11eb-962f-ddcaf20989ea.png)
![image](https://user-images.githubusercontent.com/67450413/120432313-bac60000-c3b4-11eb-9a33-aef16c32b09b.png)


# Input νκ·Έμ type μμ±
: μλ ₯ λ°μ΄ν°μ νμμ μ ν΄ μ€λλ€.
ex) <input type="some thing">

![image](https://user-images.githubusercontent.com/67450413/120432775-58b9ca80-c3b5-11eb-9428-9cf06cf2f7c5.png)
![image](https://user-images.githubusercontent.com/67450413/120432836-6ff8b800-c3b5-11eb-91b7-bd7f9fed1c3a.png)

# label νκ·Έ
: μ λͺ© μμλ₯Ό λ§λλ νκ·Έμ΄λ€.
```html
<input type="checkbox" id="user-agreement" />
<label for="user-agreement">λμνμ­λκΉ?</label>


<label><input type="checkbox" />λμνμ­λκΉ?</label>
```
- μμ λκ°λ κ°μ κΈ°λ₯μ νλ€.
- `λμ νμ­λκΉ?` λΌλ νμ€νΈ ν΄λ¦­μ checkboxμ μ²΄ν¬ νμλ¨

# textarea
: μ¬λ¬ μ€μ μΌλ° νμ€νΈ μμμ΄λ€.
- νμ€νΈ λ°μ€λ₯Ό λ§λ€ μ μκ³ , `placeholder` μμ±μ μ΄μ©νμ¬ hintλ₯Ό λ§λ€μ΄ λΌ μ μλ€!
- hintλ νμ€νΈ λ°μ€ μλ ₯ μ μ λ―Έλ¦¬ λνλ μλ κΈμλ₯Ό λ§νλ©° ν΄λ¦­ μ μ¬λΌμ§λ€.

# fieldset, legend νκ·Έ
: κ°μ λͺ©μ μ μμμ κ·Έλ£Ήν(fielset)νμ¬ μ λͺ©(legend)μ μ§μ ν΄ μ€λ€.
```html
<form>
  <fieldset>
    <legend>Coffee Size</legend>
    <label>
        <input type="radio" name="size" value="tall" />
        Tall
    </label>
    <label>
        <input type="radio" name="size" value="grande" />
        Grande
    </label>
    <label>
        <input type="radio" name="size" value="venti" />
        Venti
    </label>
  </fieldset>
</form>
```

![image](https://user-images.githubusercontent.com/67450413/120490769-a523fb00-c3f3-11eb-9448-6d6da4276760.png)
- fieldset: κ² νλλ¦¬ λ§λ€μ΄ μ€
- legend: μ λͺ© μ¦, coffee size λΆλΆμ ν΄λΉν¨

# select, option, optgroup νκ·Έ
: μ²΄ν¬λ°μ€κ° μλ μ¬λ¬κ°μ§ μ νμ°½μ λ§λ€ μ μλ€.
```html
  <select>
  <optgroup label="Coffee">
    <option>Americano</option>
    <option>Caffe Mocha</option>
    <option label="Cappuccino" value="Cappuccino"></option>
  </optgroup>
  <optgroup label="Latte" disabled>
    <option>Caffe Latte</option>
    <option>Vanilla Latte</option>
  </optgroup>
  <optgroup label="Smoothie">
    <option>Plain</option>
    <option>Strawberry</option>
    <option>Banana</option>
    <option>Mango</option>
  </optgroup>
</select>
```
- select: μ΅μμ μ ννλ λ©λ΄, κ°μ₯ ν° νλλ¦¬
- option: μ νμ°½μμ index μ­ν , μ¦ μ νμ§λ₯Ό μ§μ ν  μ μμ
- optgroup: optionμ νΉμ  groupμΌλ‘ λ¬Άμ μ μμ

# datalist νκ·Έ
```html
<input type="text" list="fruits">

<datalist id="fruits">
  <option>Apple</option>
  <option>Orange</option>
  <option>Banana</option>
  <option>Mango</option>
  <option>Fineapple</option>
</datalist>
```
- input νκ·Έλ₯Ό text νμμΌλ‘ μ§μ ν΄ textλ₯Ό μ½μ ν  μ μλ λ°μ€ μ€μ 
- datalistμ `id`μ inputμ `list`λ₯Ό κ°μ μ΄λ¦μΌλ‘ μ°λν¨
- text λ°μ€λ₯Ό ν΄λ¦­νλ©΄ datalistμ λ΄μ©λ€μ΄ μλ μμ± λλ κΈ°λ₯μ μ κ³΅

# progress
: μμμ μλ£ μ§νλ₯ μ νμ (λ‘λ© λ°)
- js νμ© μ μ΄ λ¨μλ‘ μ¦κ°νλ λ‘λ©λ° κ΅¬ν κ°λ₯
                   
   
