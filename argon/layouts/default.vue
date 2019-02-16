<template>
  <div>
   <headroom>
    <header class="header-global">
        <base-nav class="navbar-main" type="transparent" effect="dark" expand>
            <nuxt-link slot="brand" class="navbar-brand" to="/">Strainovic IT</nuxt-link>
            <div class="row" slot="content-header" slot-scope="{closeMenu}">
                <div class="col-6 collapse-brand">
                    <nuxt-link to="/">Strainovic IT</nuxt-link>
                </div>
                <div class="col-6 collapse-close">
                    <close-button @click="closeMenu"></close-button>
                </div>
            </div>

            <ul class="navbar-nav navbar-nav-hover align-items-lg-center ml-lg-auto">
            <!-- <ul class="navbar-nav navbar-nav-hover align-items-lg-center ml-lg-auto"> -->
               <base-dropdown tag="li" class="nav-item">
                    <a slot="title" href="#" class="nav-link" data-toggle="dropdown" role="button">
                        <i class="ni ni-spaceship"></i>
                        <span class="nav-link-inner--text">Dienstleistungen</span>
                    </a>
                    <nuxt-link :to="{name: 'argon-demo-landing'}" class="dropdown-item">Übersicht</nuxt-link>
                    <nuxt-link :to="{name: 'argon-demo-landing'}" class="dropdown-item">Web</nuxt-link>
                    <nuxt-link :to="{name: 'argon-demo-profile'}" class="dropdown-item">Domain</nuxt-link>
                    <nuxt-link :to="{name: 'argon-demo-login'}" class="dropdown-item">Hosting</nuxt-link>
                    <nuxt-link :to="{name: 'argon-demo-register'}" class="dropdown-item">Shops</nuxt-link>
               </base-dropdown>
               <base-dropdown tag="li" class="nav-item">
                    <a slot="title" href="#" class="nav-link" data-toggle="dropdown" role="button">
                        <i class="ni ni-single-02"></i>
                        <span class="nav-link-inner--text">Über mich</span>
                    </a>
                    <nuxt-link :to="{name: 'argon-demo-landing'}" class="dropdown-item">Personalien</nuxt-link>
                    <nuxt-link :to="{name: 'argon-demo-profile'}" class="dropdown-item">Skills</nuxt-link>
                    <nuxt-link :to="{name: 'argon-demo-login'}" class="dropdown-item">Ausbildung</nuxt-link>
                    <nuxt-link :to="{name: 'argon-demo-register'}" class="dropdown-item">Jobs</nuxt-link>
                </base-dropdown>
               <base-dropdown tag="li" class="nav-item">
                    <a slot="title" href="#" class="nav-link" data-toggle="dropdown" role="button">
                        <i class="ni ni-collection"></i>
                        <span class="nav-link-inner--text">Projekte</span>
                    </a>
                        <nuxt-link :to="{name: 'argon-demo-landing'}" class="dropdown-item">Webseiten</nuxt-link>
                        <nuxt-link :to="{name: 'argon-demo-profile'}" class="dropdown-item">Diverse</nuxt-link>
                </base-dropdown>
               <base-dropdown tag="li" class="nav-item mr-lg-n3">
                    <a slot="title" href="#" class="nav-link" data-toggle="dropdown" role="button">
                        <i class="ni ni-email-83"></i>
                        <span class="nav-link-inner--text">Kontakt</span>
                    </a>
                        <nuxt-link :to="{name: 'argon-demo-landing'}" class="dropdown-item">Kontaktformular</nuxt-link>
                        <nuxt-link :to="{name: 'argon-demo-profile'}" class="dropdown-item">Konktaktdaten</nuxt-link>
                        <nuxt-link :to="{name: 'argon-demo-profile'}" class="dropdown-item">Karte</nuxt-link>
                </base-dropdown>
            </ul>
       </base-nav>
    </header>
   </headroom>
    <main>
        <nuxt />
    </main>
     <footer class="footer has-cards">
        <div class="container container-lg">
            <div class="row">
                <div class="col-md-6 mb-5 mb-md-0">
                    <div class="card card-lift--hover shadow border-0">
                        <nuxt-link :to="{name: 'argon-demo-landing'}" title="Landing Page">
                            <img v-lazy="'/argon/img/theme/landing.jpg'" class="card-img">
                        </nuxt-link>
                    </div>
                </div>
                <div class="col-md-6 mb-5 mb-lg-0">
                    <div class="card card-lift--hover shadow border-0">
                        <nuxt-link :to="{name: 'argon-demo-profile'}" title="Profile Page">
                            <img v-lazy="'/argon/img/theme/profile.jpg'" class="card-img">
                        </nuxt-link>
                    </div>
                </div>
            </div>
        </div>
        <div class="container">
            <div class="row row-grid align-items-center my-md">
                <div class="col-lg-6">
                    <h3 class="text-primary font-weight-light mb-2">Vielen Dank für deine Unterstützung!</h3>
                    <h4 class="mb-0 font-weight-light">Folge mir auf einer dieser Plattformen.</h4>
                </div>
                <div class="col-lg-6 text-lg-center btn-wrapper">
                    <a target="_blank" href="https://twitter.com/Strainovic_IT"
                       class="btn btn-neutral btn-icon-only btn-twitter btn-round btn-lg" data-toggle="tooltip"
                       title="Folge mir auf Twitter">
                        <i class="fa fa-twitter"></i>
                    </a>
                    <a target="_blank" href="https://www.facebook.com/StrainovicIT/"
                       class="btn btn-neutral btn-icon-only btn-facebook btn-round btn-lg" data-toggle="tooltip"
                       title="Like mich auf Facebook">
                        <i class="fa fa-facebook-square"></i>
                    </a>
                    <a target="_blank" href="https://www.instagram.com/strainovic_it/"
                       class="btn btn-neutral btn-icon-only btn-instagram btn-lg btn-round" data-toggle="tooltip"
                       title="Folge mir auf Instagram">
                        <i class="fa fa-instagram"></i>
                    </a>
                    <a target="_blank" href="https://ch.linkedin.com/in/goran-strainovic"
                       class="btn btn-neutral btn-icon-only btn-linkedin btn-round btn-lg" data-toggle="tooltip"
                       title="Folge mir auf LinkedIn">
                        <i class="fa fa-linkedin"></i>
                    </a>
                    <a target="_blank" href="https://github.com/gstrainovic"
                       class="btn btn-neutral btn-icon-only btn-github btn-round btn-lg" data-toggle="tooltip"
                       title="Spendiere mir einen Stern auf Github">
                        <i class="fa fa-github"></i>
                    </a>
                     <a target="_blank" href="https://www.xing.com/profile/Goran_Strainovic"
                       class="btn btn-neutral btn-icon-only btn-xing btn-round btn-lg" data-toggle="tooltip"
                       title="Folge mir auf Xing">
                        <i class="fa fa-xing"></i>
                    </a>
                </div>
            </div>

          </ul>
            <hr>
            <div class="row align-items-center justify-content-md-between">
                <div class="col-md-6">
                    <div class="copyright">
                        &copy; 2018
                        <a href="https://www.creative-tim.com" target="_blank">Creative Tim</a>.
                    </div>
                </div>
                <div class="col-md-6">
                    <ul class="nav nav-footer justify-content-end">
                        <li class="nav-item">
                            <a href="https://www.creative-tim.com" class="nav-link" target="_blank">Creative Tim</a>
                        </li>
                        <li class="nav-item">
                            <a href="https://www.creative-tim.com/presentation" class="nav-link" target="_blank">About
                                Us</a>
                        </li>
                        <li class="nav-item">
                            <a href="http://blog.creative-tim.com" class="nav-link" target="_blank">Blog</a>
                        </li>
                        <li class="nav-item">
                            <a href="https://github.com/creativetimofficial/argon-design-system/blob/master/LICENSE.md"
                               class="nav-link" target="_blank">MIT License</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
  </div>
</template>

<script>
import BaseNav from "~/components/argon/BaseNav";
import BaseDropdown from "~/components/argon/BaseDropdown";
import CloseButton from "~/components/argon/CloseButton";
import { headroom } from 'vue-headroom';

export default {
  components: {
    BaseNav,
    CloseButton,
    BaseDropdown,
    headroom
  }
};
</script>
<style>
.headroom--not-top {
    padding-top: 0;
    padding-bottom: 0;
}
@media (min-width: 992px){
  .navbar-main {
      padding: 0;
  }
}
</style>
