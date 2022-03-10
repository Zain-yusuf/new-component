<template>
  <div>
    <div class="main" v-for="name in names" :key="name.id">
      <h1>{{ name.name }}</h1>
      <ul class="list">
        <li>{{ name.Father_name }}</li>
        <li>{{ name.class }}</li>
        <li>{{ name.gmail }}</li>
        <li>{{ name.Adress }}</li>
      </ul>
    </div>
    <div>
      <h2>{{ array }}</h2>
    </div>
  </div>
</template>

<script>
export default {
  name: "child",
  props: {
    array: Array,
  },
  data() {
    return {
      names: [
        {
          name: "zain",
          Father_name:"Father name:  yusuf shaheen",
          class: "Class:  1st year",
          gmail: "Gmail:  zain.yusuf.786@gmail.com",
          Adress: "Adress:  24/wb vehari",
        },
        {
          name: "sufyan",
          Father_name: "Father name:  yusuf",
          class: "Class:  PHD se bhi oper",
          gmail: "Gmail:  sufyan.yusuf.786@gmail.com",
          Adress: "Adress:  24/wb vehari",
        },
        {
          name: "bilal",
          Father_name: "Father name:  Iqbal",
          class: "Class:  2nd year",
          gmail: "Gmail:  bilal.786@gmail.com",
          Adress: "Adress: 24/wb vehari",
        },
        {
          name: "numan",
          Father_name: "Father name:  pta nai",
          class: "class:  2nd year",
          gmail: "Gmail:  numan.786@gmail.com",
          Adress: "Adress:  24/wb vehari",
        },
        {
          name: "Abdullah",
          Father_name: "Father name:  Iqbal",
          class: "class:  PHD",
          gmail: "Gmail:  abdullah.786@gmail.com",
          Adress: "Adress:  24/wb vehari",
        },
      ],
    };
  },
};
</script>

<style sscoped>
li {
  list-style-type: none;
}
div > h1 {
  text-transform: uppercase;
}
.main {
    border: 2px solid red;
  width: 30%;
  margin-left: 7%;
}
.list{
    text-align: left;
}
</style>