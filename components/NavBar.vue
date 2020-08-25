<template>
  <div class="pb-5">
    <b-navbar fixed="top" toggleable="sm" type="dark" variant="dark">
      <b-container>
        <b-navbar-brand to="/" href="#">Home</b-navbar-brand>
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav class="custom-links">
            <b-nav-item href="#" to="/programming">Programming</b-nav-item>
            <b-nav-item href="#" to="/education">Education</b-nav-item>
            <b-nav-item href="#" to="/authorList">Author List</b-nav-item>
          </b-navbar-nav>
          <b-navbar-nav class="ml-auto custom-links">
            <b-nav-item href="#" to="/login" class="ml-auto">Log In</b-nav-item>
          </b-navbar-nav>
        </b-collapse>
      </b-container>
    </b-navbar>
  </div>
</template>

<style scopde>
.custom-links a {
  color: white !important;
}
</style>
