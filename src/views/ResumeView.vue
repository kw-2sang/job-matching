<script setup>
import Header from '@/components/Header.vue'
</script>
<template>
  <div class="container">
    <Header />
    <h1 class="mb-3 text-center">지원서 작성</h1>
    <h4 class="mb-3">인적 사항</h4>
    <form class="needs-validation" novalidate>
      <div class="row g-3">
        <div class="col-sm-6">
          <label for="firstName" class="form-label">한글 성명</label>
          <input type="text" class="form-control" id="koName" placeholder="" value="" required>
          <div class="invalid-feedback">
            한글 성명을 작성해주세요.
          </div>
        </div>

        <div class="col-sm-6">
          <label for="lastName" class="form-label">영문 성명</label>
          <input type="text" class="form-control" id="enName" placeholder="" value="" required>
          <div class="invalid-feedback">
            영문 성명을 작성해주세요.
          </div>
        </div>

        <div class="col-6">
          <label for="email" class="form-label">이메일</label>
          <input type="email" class="form-control" id="email" placeholder="myemail@kw.ac.kr">
          <div class="invalid-feedback">
            이메일을 작성해주세요.
          </div>
        </div>

        <div class="col-6">
          <label for="phone" class="form-label">연락처</label>
          <input type="phone" class="form-control" id="phone" placeholder="010-1234-1234">
          <div class="invalid-feedback">
            연락처를 작성해주세요.
          </div>
        </div>

        <div class="col-12">
          <label for="address" class="form-label">주소</label>
          <input type="text" class="form-control" id="address" placeholder="서울특별시 노원구 광운로 20" required>
          <div class="invalid-feedback">
            주소를 입력해주세요.
          </div>
        </div>

        <hr class="my-4">
        
        <h4 class="mb-3">나의 기술 스택</h4>
        <div class="form-check form-check-inline">
          <input type="checkbox" class="form-check-input" name="skills" id="skill1">
          <label class="form-check-label" for="skill1">Vue</label>
        </div>
        <div class="form-check form-check-inline">
          <input type="checkbox" class="form-check-input" name="skills" id="skill2">
          <label class="form-check-label" for="skill2">Bootstrap</label>
        </div>
        <div class="form-check form-check-inline">
          <input type="checkbox" class="form-check-input" name="skills" id="skill3">
          <label class="form-check-label" for="skill3">D3.js</label>
        </div>
        <div class="col-12">
          <label for="addskill" class="form-label">나는 이것도 할 수 있다(자유작성)</label>
          <input type="text" class="form-control" id="addskill" placeholder="React, JS ..." required>
        </div>
      </div>

      <hr class="my-4">

      <h4 class="mb-3">자기소개서</h4>
      <div class="card" style="height: 50vh">
        <div class="card-body">
          기업 자유 양식
        </div>
      </div>

      <hr class="my-4">

      <button class="w-100 btn btn-primary btn-lg mb-5" type="submit">작성 완료</button>
    </form>

    <div class="row pb-5">
      <div class="col">
        <RouterLink to="/detail" type="button" class="btn btn-secondary" style="float: left;">이전페이지</RouterLink>
      </div>
    </div>
  </div>
</template>