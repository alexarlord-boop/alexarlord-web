<template>
  <nav class="navbar navbar-expand-lg bg-body-tertiary" style="box-shadow: rgba(225,225,203,0.58) 2px 5px 20px">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">alexarlord |</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">

          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              💻 Featured Projects
            </a>
            <ul class="dropdown-menu">
              <li><a class="dropdown-item" href="#ml-projects">ML <span class="rounded-pill text-bg-warning p-1"> in progress</span></a></li>
              <li><a class="dropdown-item" href="#cloud-projects">DevOps</a></li>
              <li><a class="dropdown-item" href="#software-projects">Software</a></li>
<!--              <li><hr class="dropdown-divider"></li>-->
              <li><a class="dropdown-item" href="#uni-basics-projects">First Steps</a></li>
            </ul>
          </li>

          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="https://github.com/alexarlord-boop" target="_blank">GitHub</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="https://www.linkedin.com/in/aleksandr-petrunin-b4b720259/" target="_blank">LinkedIn</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navbar"
}
</script>

<style scoped>

</style>