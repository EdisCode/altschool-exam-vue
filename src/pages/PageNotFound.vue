<template>
<div className="page-not-found">
      <h1>404</h1>
      <div>
        <h2>We can't find that page.</h2>
        <p>
          Maybe this page moved? Got deleted? Is hiding out in quarantine? Never
          existed in the first place?
        </p>
        <p>We do apologise on it's behalf.</p>
        <div>
          <p>Let's go </p>
          <router-link className="link active" to="/">"Home"</router-link>
          <p> and try from there.</p>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'PageNotFound'
}</script>