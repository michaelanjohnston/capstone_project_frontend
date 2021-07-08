<template>
  <div id="app">
    <!-- Page Wrapper -->
    <div id="page-wrapper">
      <!-- Header -->
      <header id="header" class="alt">
        <h1><a href="index.html">Daily Inspirational Quote</a></h1>
        <nav id="nav">
          <ul>
            <li class="special">
              <a href="#menu" class="menuToggle"><span>Menu</span></a>
              <div id="menu">
                <ul>
                  <li><a href="/about">About</a></li>
                  <li><a href="/signup">Sign Up</a></li>
                  <li><a href="/login">Log In</a></li>
                  <li><a href="/logout">Log In</a></li>
                </ul>
              </div>
            </li>
          </ul>
        </nav>
      </header>

      <!-- Banner -->
      <section id="banner">
        <div class="inner">
          <h2>Daily Inspirational Quote</h2>
        </div>
        <a href="#one" class="more scrolly">Past Posts</a>
      </section>

      <!-- One -->
      <section id="one" class="wrapper style1 special"></section>

      <!-- Two -->
      <section id="two" class="wrapper alt style2">
        <section class="spotlight"></section>
        <section class="spotlight"></section>
        <section class="spotlight"></section>
      </section>

      <!-- Three -->
      <router-view />
      <!-- Footer -->
      <footer id="footer">
        <ul class="icons">
          <li>
            <a href="#" class="icon brands fa-twitter"><span class="label">Twitter</span></a>
          </li>
          <li>
            <a href="#" class="icon brands fa-facebook-f"><span class="label">Facebook</span></a>
          </li>
          <li>
            <a href="#" class="icon brands fa-instagram"><span class="label">Instagram</span></a>
          </li>
          <li>
            <a href="#" class="icon brands fa-dribbble"><span class="label">Dribbble</span></a>
          </li>
          <li>
            <a href="#" class="icon solid fa-envelope"><span class="label">Email</span></a>
          </li>
        </ul>
        <ul class="copyright">
          <li>&copy; Untitled</li>
          <li>
            Design:
            <a href="http://html5up.net">HTML5 UP</a>
          </li>
        </ul>
      </footer>
    </div>
  </div>
</template>

<style></style>
