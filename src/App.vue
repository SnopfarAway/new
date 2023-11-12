<script setup lang="ts">
//import { RouterLink, RouterView } from 'vue-router'
//import HelloWorld from './components/HelloWorld.vue'
</script>

<template>

  <body>
  
  <section>
    

    <form action="/submit_form" method="post">
      <section>  
        <div>
          <label for="fio" style="float: left">ФИО</label>
          <input type="text" id="fio" name="fio" placeholder="Иванов Иван Иванович" readonly><br>
        </div>
        <div>
          <label for="email" style="float: left">Email</label>
          <input type="email" id="mail" name="mail" placeholder="ivanivanov@gmail.com"><br>
        </div>
        <div>
          <label for="phone" style="float: left">Телефон</label>
          <input type="text" id="phone" name="phone" placeholder="+7 (777) 777 77-77"><br>
        </div>
      </section>
      

      <section>
        <h2>Адрес доставки</h2>
      <div>
        <div style="display: inline-block; margin: 10px; width: 20%;">
        <label for="zip" style="">Индекс</label>
        <input type="text" id="zip" name="zip" placeholder="400003"><br>
      </div>
      <div style="display: inline-block; margin: 10px; width: 70%;">
        <label for="city">Город</label>
        <input type="text" id="city" name="city" placeholder="г. Волгоград" style=""><br>
      </div>
      </div>
      <div style="display: inline-block; margin: 10px; width: 70%;">
        <label for="street">Улица</label>
        <input type="text" id="street" name="street" placeholder="ул. Штеменко 23"><br>
      </div>
      <div style="display: inline-block; margin: 10px; width: 20%;">
        <label for="building">Корпус</label>
        <input type="text" id="building" name="building" placeholder="2Б" style=""><br>
      </div>
      <div style="display: inline-block; margin: 10px; width: 20%;">
        <label for="appartments">Квартира</label>
        <input type="text" id="appartments" name="appartments" placeholder="50"><br>
      </div>
      <div style="display: inline-block; margin: 10px; width: 70%;">
        <label for="subscribe" style="margin: 30px;">Частный дом</label>
        <input type="checkbox" id="subscribe" name="subscribe" value="yes">
      </div>
      </section>
      
        <button type="submit">Редактировать данные</button>
    </form>
    </section>
  
  <div class="rightbuttons">
    <button class="rightbuttons-elements" type="submit">Персональные данные</button>
    <button class="rightbuttons-elements" type="submit">Истории заказов</button>
    <button class="rightbuttons-elements" type="submit">Смена пароля</button>
  </div>
  </body>
</template>

<style>


body {
  max-width: 1280px;
    font-family: Arial, sans-serif;
    margin: 10px;
    padding: 10px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #f2f2f2;
}
form {
    width: 440px;
    padding: 20px;
    background-color: #fff;
    border-radius: 5px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    text-align: center;
}
input[type="text"], input[type="email"], input[type="number"], input[type="file"] {
    width: 100%;
    margin: 2px 0;
    padding: 10px;
    box-sizing: border-box;
    border: 1px solid #ccc;
    border-radius: 5px;
}
input[type="file"] {
    border: none;
}
input[type="checkbox"] {
    margin-right: 5px;
}
button {
  margin: 10px;
  width: 214px;
  height: 44px;
  padding: 10px 20px;
  background-color: #FFC94F;
  color: #464855;
  font-weight: 700 ;
  font-size: 14px ;
  border: none;
  border-radius: 2px;
  cursor: pointer;
}
.rightbuttons{
  margin: 30px;
  height: 70px;
  width: 100px;
  position: relative;
}
.rightbuttons-elements{
  width: 242px;
  height: 53px;
  margin: 6px;
  background-color: #3D4F64;
  color: white;
  font-size: 16px ;
  font-weight: 700 ;
  border-radius: 2px;
}
.block {
  display: inline-block;
  margin: 10px;
}
</style>