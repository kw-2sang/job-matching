<script setup>
import Header from '@/components/Header.vue'
</script>
<template>
  <div class="container">
    <Header />
    <div class="row">
      <div class="col-10">
        <div>
          <h1 style="font-weight: 600; display: inline;">OO기업</h1>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
          <h3 style="display: inline;">IT | 중견기업</h3>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
          <h5 style="display: inline;">신입</h5>
        </div>
        <div class="row my-3">
          <div class="col-1">&nbsp;</div>
          <div class="col-11">
            <ul>
              <li class="mb-1">마감일 : 2022년 12월 16일 23:59</li>
              <li class="mb-1">채용형태 : 신입 | 서류전형 인적성검사 실무면접 임원면접</li>
              <li class="mb-1">기술스택 : Vue Bootstrap D3.js</li>
            </ul>
          </div>
        </div>
        <div class="card" style="height: 50vh">
          <div class="card-body">
            기업 자유 양식
          </div>
        </div>
      </div>
      <div class="col-2">
        <div class="card" style="height: 70vh">
          <div class="card-body">
            비슷한 기업 리스트
          </div>
        </div>
      </div>
    </div>
    <div class="row my-5">
      <div class="col">
        <RouterLink to="/" type="button" class="btn btn-secondary" style="float: left;">이전페이지</RouterLink>
        <RouterLink to="/resume" type="button" class="btn btn-secondary" style="float: right;">다음페이지</RouterLink>
      </div>
    </div>
  </div>
</template>