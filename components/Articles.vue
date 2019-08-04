<template>
  <div class="a-content">
    <div v-for="(item, index) in items" :key="index">
      <div>
        {{item.question}}
      </div>
      <a-checkbox-group @change="onChange">
        <a-row>
          <a-col :span="24"><a-radio>(A)</a-radio><span>Hello</span></a-col>
          <a-col :span="24"><a-radio>(B)</a-radio></a-col>
          <a-col :span="24"><a-radio>(C)</a-radio></a-col>
          <a-col :span="24"><a-radio>(D)</a-radio></a-col>
        </a-row>
      </a-checkbox-group>
    </div>
  </div>
</template>
<script>
export default {
  data: {
    items: [
      {question:'Hello', list: ['ABC','ABC','CDS','XXc']},
      {question:'Hello', list: ['ABC','ABC','CDS','XXc']}
    ]
  },
  methods: {
    onChange (checkedValues) {
      console.log('checked = ', checkedValues)
    },
  },
}
</script>
<style>
  .a-content{

  }
</style>
