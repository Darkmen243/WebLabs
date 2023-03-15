# lab2
##checkbox.vue

![image](https://user-images.githubusercontent.com/46415000/225363379-0b2dbab9-fb23-453d-a8b3-8990f33b1f90.png)
![image](https://user-images.githubusercontent.com/46415000/225363439-f6464ec0-214c-47d4-a126-7c9341199534.png)

Этот компонент представляет из себя чекбокс, при нажатии на который он меняет цвет и изображение внутри.
Данный компонент содержит prop - value типа boolean, обозначающий текущее состояние чекбокса и событие "change", которое отвечают за изменение чекбокса в методе "check".
```
 model: {
    prop: "value",
    event: "change"
  },
  props: {
    value: Boolean
  },
  methods: {
    check: function () {
      this.$emit("change", !this.value);
    }
  }
```
Импорт компонента и использование компонента производятся с помощью данных команд
```
import CheckBox from './components/Checkbox.vue'

 <CheckBox v-model="v-model-name"></CheckBox>
```
