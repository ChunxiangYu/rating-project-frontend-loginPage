<template>
  <form class="login-form">
    <div id="topLogo">
      <img id="logo" alt="" src="/EduSourceLogo.png" />
    </div>
    <form class="input-form">
      <ul class="wrapper">
        <li id="welcome">
          <label class="welcome">Welcome back,</label>
          <label class="welcome">Login here</label>
        </li>
        <li id="emailInput">
          <label>
            <input
              class="inputLine"
              placeholder="Email"
              type="text"
              v-model="email"
            />
          </label>
          <label class="notice">Inactive</label>
        </li>
        <li id="passwordInput">
          <label>
            <input
              class="inputLine"
              placeholder="Password"
              type="password"
              v-model="password"
              @keypress.enter="login"
            />
          </label>
          <label class="notice">Hover</label>
        </li>
      </ul>
    </form>
    <div>
      <div class="actions">
        <button id="loginButton" type="button" @click="login">LOG IN</button>
      </div>
      <div class="actions">
        <button id="signupButton" type="button" @click="signUp">SIGN UP</button>
      </div>
    </div>
  </form>
</template>

<style lang="less" src="./login.less"></style>
<script lang="ts" src="./login.ts"></script>
