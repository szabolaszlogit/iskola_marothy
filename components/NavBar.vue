<template>
  <b-navbar toggleable="lg" type="dark" variant="dark">
    <b-navbar-brand href="#">Maróthy Iskola</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item href="/">Kezdőlap</b-nav-item>
        <b-nav-item href="/adatok">Adatok, kapcsolat</b-nav-item>
        <b-nav-item href="/marothy">Névadónk</b-nav-item>
        <b-nav-item href="/marothy-dij">Maróthy-díj</b-nav-item>
        <b-nav-item href="/alapitvany">Alapítvány</b-nav-item>
        <b-nav-item href="/kozzeteteli">Közzétételi lista</b-nav-item>        
        <b-nav-item href="/tantervek">Tantervek</b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">

         <b-button
          href="https://klik033463001.e-kreta.hu/Adminisztracio/Login"
          target="_blank"
          variant="success"
          class="m-2"
          >Kréta</b-button
        >         
        <b-button
          href="https://www.facebook.com/MarothyJanosAltIsk/"
          target="_blank"
          variant="primary"
          class="m-2"
          >Facebook</b-button
        >
        <b-button
          href="https://www.youtube.com/user/Rozsaly"
          target="_blank"
          variant="primary"
          class="m-2"
          >Youtube</b-button
        >
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<style></style>
