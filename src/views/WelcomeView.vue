<script setup>
import { ref } from 'vue'
import { RouterLink } from 'vue-router'
const job_detail = ref([])

const list_developer = ['Frontend', 'Backend', 'Full Stack', 'AI ML', 'System']
const list_marketing = ['국내', '해외', 'B2C', 'B2B']
const list_finance = ['기타1', '기타2', '기타3', '기타4']
const list_engineer = ['기타1', '기타2', '기타3', '기타4']

const lists = [list_developer, list_marketing, list_finance, list_engineer]

const change_list = (num) => {
  job_detail.value = lists[num]
}
</script>

<template>
  <div class="container" style="width: 100%;">
    <div class="my-5">
      <h1>환영합니다!</h1><h3>당신의 업무 분야를 선택해주세요.</h3>
    </div>

    <div class="row my-5">
      <div class="col-6">
        <div class="list-group">
          <a href="#" class="list-group-item list-group-item-action" @click="change_list(0)">Developer</a>
          <a href="#" class="list-group-item list-group-item-action" @click="change_list(1)">Marketing</a>
          <a href="#" class="list-group-item list-group-item-action" @click="change_list(2)">Finance</a>
          <a href="#" class="list-group-item list-group-item-action" @click="change_list(3)">Engineer</a>
        </div>
      </div>
      <div class="col-6">
        <div class="list-group">
          <a v-for="item in job_detail" href="#" class="list-group-item list-group-item-action">{{ item }}</a>
        </div>
      </div>
    </div>
    <div class="row my-5">
      <div class="col">
        <RouterLink to="/" type="button" class="btn btn-secondary" style="float: right;">다음페이지</RouterLink>
      </div>
    </div>
  </div>
</template>