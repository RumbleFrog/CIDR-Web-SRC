<template>
  <section class="hero is-large animated fadeIn">
    <div class="hero-body">
      <div class="container">
        <div class="columns">
          <div class="column is-one-third">
            <h1 class="title">Documentation (<em>WIP</em>)</h1>
            <nav class="breadcrumb" aria-label="breadcrumbs">
              <ul>
                <li><router-link :to="{ name: 'Index', params: {} }">CIDR Blocker</router-link></li>
                <li class="is-active"><router-link :to="{ name: 'Documentation', params: {} }">Documentation</router-link></li>
              </ul>
            </nav>
            <aside class="menu">
              <p class="menu-label">
                General
              </p>
              <ul class="menu-list">
                <li><router-link :to="{ name: 'Documentation', params: {} }" exact-active-class="is-active">Introduction</router-link></li>
              </ul>
              <p class="menu-label">
                Setup
              </p>
              <ul class="menu-list">
                <li><router-link :to="{ name: 'Documentation/Setup/Installation', params: {} }" exact-active-class="is-active">Installation</router-link></li>
                <li><router-link :to="{ name: 'Documentation/Setup/Troubleshooting', params: {} }" exact-active-class="is-active">Troubleshooting</router-link></li>
              </ul>
            </aside>
          </div>
          <div class="column">
            <div class="box">
              <keep-alive><router-view></router-view></keep-alive>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
