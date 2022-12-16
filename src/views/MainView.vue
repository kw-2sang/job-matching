<script setup>
import Header from '@/components/Header.vue'
</script>
<template>
  <div class="container">
    <Header />
    <div class="row">
      <div class="col-2">
        <p class="text-center mt-3">선호하는 기술 스택</p>
        <div class="list-group">
          <a href="#" class="list-group-item list-group-item-action">React</a>
          <a href="#" class="list-group-item list-group-item-action">Vue</a>
          <a href="#" class="list-group-item list-group-item-action">Angular</a>
          <a href="#" class="list-group-item list-group-item-action">Vanilla JS</a>
        </div>
        <p class="text-center mt-3">비선호 기술 스택</p>
        <div class="list-group">
          <a href="#" class="list-group-item list-group-item-action">React</a>
          <a href="#" class="list-group-item list-group-item-action">Vue</a>
          <a href="#" class="list-group-item list-group-item-action">Angular</a>
          <a href="#" class="list-group-item list-group-item-action">Vanilla JS</a>
        </div>
      </div>
      <div class="col-10">
        <div class="card mt-3 mb-5">
          <div class="row">
            <div class="col-6 card-body text-center">
              <div class="form-check form-check-inline">
                <input class="form-check-input" type="radio" name="companySize" id="large" value="large">
                <label class="form-check-label" for="large">대기업</label>
              </div>
              <div class="form-check form-check-inline">
                <input class="form-check-input" type="radio" name="companySize" id="regular" value="regular">
                <label class="form-check-label" for="regular">중견기업</label>
              </div>
              <div class="form-check form-check-inline">
                <input class="form-check-input" type="radio" name="companySize" id="small" value="small">
                <label class="form-check-label" for="small">중소기업</label>
              </div>
            </div>
            <div class="col-6 card-body text-center">
              <div class="form-check form-check-inline">
                <input class="form-check-input" type="radio" name="companyTypes" id="it" value="it">
                <label class="form-check-label" for="it">IT</label>
              </div>
              <div class="form-check form-check-inline">
                <input class="form-check-input" type="radio" name="companyTypes" id="finance" value="finance">
                <label class="form-check-label" for="finance">금융</label>
              </div>
              <div class="form-check form-check-inline">
                <input class="form-check-input" type="radio" name="companyTypes" id="public" value="public">
                <label class="form-check-label" for="public">공공</label>
              </div>
            </div>
          </div>
        </div>
        기업 리스트
        <div class="card mb-1">
          <div class="card-body">
            OO기업 | Web Developer | React Bootstrap | 12월 16일
          </div>
        </div>
        <div class="card mb-1">
          <div class="card-body">
            OO기업 | Web Developer | React Bootstrap | 12월 16일
          </div>
        </div>
        <div class="card mb-1">
          <div class="card-body">
            OO기업 | Web Developer | React Bootstrap | 12월 16일
          </div>
        </div>
        <div class="card mb-1">
          <div class="card-body">
            OO기업 | Web Developer | React Bootstrap | 12월 16일
          </div>
        </div>
        <div class="card mb-1">
          <div class="card-body">
            OO기업 | Web Developer | React Bootstrap | 12월 16일
          </div>
        </div>
      </div>
    </div>
    <div class="row my-5">
      <div class="col">
        <RouterLink to="/welcome" type="button" class="btn btn-secondary" style="float: left;">이전페이지</RouterLink>
        <RouterLink to="/detail" type="button" class="btn btn-secondary" style="float: right;">다음페이지</RouterLink>
      </div>
    </div>
  </div>
</template>