# CSS\_\_Watermelon

## Авторське право:

[Фрілансер по життю](https://www.youtube.com/c/freelancerlifestyle)
https://codepen.io/FreelancerLifeStyle/pen/GRGWVpb

```css
/_ Встановлюємо розмір контейнера та властивості для 3D-перспективи _/
.body {
width: 650px; /_ Ширина контейнера _/
height: 500px; /_ Висота контейнера _/
perspective: 400px; /_ Встановлюємо перспективу для 3D ефекту _/
display: flex; /_ Використовуємо flexbox для центрованого вирівнювання _/
justify-content: center; /_ Горизонтальне вирівнювання по центру _/
align-items: center; /_ Вертикальне вирівнювання по центру _/
}

/_ Оформлення елемента кавуна _/
.watermelon {
width: 510px; /_ Ширина кавуна _/
height: 250px; /_ Висота кавуна _/
overflow: hidden; /_ Приховуємо частини, що виходять за межі контейнера _/
position: relative; /_ Встановлюємо відносне позиціонування для дітей _/
transform: rotateY(-15deg) rotateZ(20deg); /_ Поворот кавуна для 3D ефекту _/
}

/_ Псевдоелемент для зеленої частини кавуна _/
.watermelon::before {
content: ""; /_ Створюємо пустий контент _/
position: absolute; /_ Абсолютне позиціонування _/
width: 500px; /_ Ширина зеленої частини _/
height: 500px; /_ Висота зеленої частини _/
bottom: 0px; /_ Вирівнювання по низу _/
right: 0px; /_ Вирівнювання по правому краю _/
border-radius: 300px 500px 330px 500px; /_ Округлення країв для форми кавуна _/
background-color: #1a360b; /_ Зелений колір шкірки кавуна _/
}

/_ Псевдоелемент для червоної частини кавуна _/
.watermelon::after {
content: ""; /_ Створюємо пустий контент _/
position: absolute; /_ Абсолютне позиціонування _/
width: 500px; /_ Ширина червоної частини _/
height: 500px; /_ Висота червоної частини _/
bottom: 10px; /_ Вирівнювання по низу з невеликим відступом _/
left: 0; /_ Вирівнювання по лівому краю _/
border-bottom: 20px solid #3d6e23; /_ Нижня рамка зелена, щоб створити край _/
background-color: rgb(153, 31, 31); /_ Червоний колір м'якоті кавуна _/
border-radius: 50%; /_ Округлення країв для форми м'якоті кавуна _/
}

/_ Загальні властивості для кісточок кавуна _/
.watermelon span {
position: absolute; /_ Абсолютне позиціонування для кожної кісточки _/
background-color: #000; /_ Чорний колір кісточок _/
width: 20px; /_ Ширина кісточок _/
height: 20px; /_ Висота кісточок _/
z-index: 2; /_ Встановлюємо кісточки поверх інших елементів _/
border-radius: 5px 5px 20px 20px; /_ Округлення країв для форми кісточок _/
}

/_ Індивідуальне позиціонування кожної кісточки _/
.watermelon span:nth-child(1) {
left: 10%; /_ Відступ зліва _/
top: 10%; /_ Відступ зверху _/
}
.watermelon span:nth-child(2) {
left: 30%;
top: 20%;
}
.watermelon span:nth-child(3) {
left: 50%;
top: 40%;
}
.watermelon span:nth-child(4) {
left: 20%;
top: 45%;
}
.watermelon span:nth-child(5) {
left: 60%;
top: 15%;
}
.watermelon span:nth-child(6) {
left: 75%;
top: 35%;
}
.watermelon span:nth-child(7) {
left: 85%;
top: 15%;
}
.watermelon span:nth-child(8) {
left: 35%;
top: 65%;
}
.watermelon span:nth-child(9) {
left: 65%;
top: 60%;
}
```

## perspective

https://css.in.ua/css/property/perspective
