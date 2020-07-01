<template>
  <div>
    <h1>{{ msg }}</h1>
    <counter />
    <ItemList />
    <!--counterを持ってくる -->
  </div>
</template>

<script>
import Counter from "./Counter.vue"; //componentを読み込む
import ItemList from "./ItemList";

export default {
  name: "HelloWorld",
  props: {
    msg: String
  },
  components: {
    //componentの登録
    Counter,
    ItemList
  }
};
</script>
