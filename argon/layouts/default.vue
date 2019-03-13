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
                    <nuxt-link to=/# class="dropdown-item">Alles aus einer Hand</nuxt-link>
                    <nuxt-link to=/# class="dropdown-item">Web</nuxt-link>
                    <nuxt-link to=#software class="dropdown-item">Software</nuxt-link>
               </base-dropdown>
               <base-dropdown tag="li" class="nav-item">
                    <a slot="title" href="#" class="nav-link" data-toggle="dropdown" role="button">
                        <i class="ni ni-single-02"></i>
                        <span class="nav-link-inner--text">Über uns</span>
                    </a>
                    <nuxt-link :to="{name: 'argon-demo-landing'}" class="dropdown-item">Über Strainovic IT</nuxt-link>
                    <div class="dropdown-divider"></div>
                    <nuxt-link :to="{name: 'argon-demo-landing'}" class="dropdown-item">Über Goran Strainovic</nuxt-link>
                    <nuxt-link :to="{name: 'argon-demo-landing'}" class="dropdown-item">Personalien</nuxt-link>
                    <nuxt-link :to="{name: 'argon-demo-profile'}" class="dropdown-item">Skills</nuxt-link>
                    <nuxt-link :to="{name: 'argon-demo-login'}" class="dropdown-item">Ausbildung</nuxt-link>
                    <nuxt-link :to="{name: 'argon-demo-register'}" class="dropdown-item">Jobs</nuxt-link>
                </base-dropdown>
               <base-dropdown tag="li" class="nav-item">
                    <a slot="title" href="#" class="nav-link" data-toggle="dropdown" role="button">
                        <i class="ni ni-collection"></i>
                        <span class="nav-link-inner--text">Portfolio</span>
                    </a>
                        <nuxt-link to=/portfolio/web class="dropdown-item">Webseiten</nuxt-link>
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
<section class="section section-shaped my-0 overflow-hidden">
            <div class="shape shape-style-3 bg-gradient-default shape-skew">
                <span></span>
                <span></span>
                <span></span>
                <span></span>
            </div>
            <div class="container pt-lg pb-300">
              <div class="row">
                    <div class="col-lg-10">
                        <h2 class="display-3 text-white">Wir freuen uns auf Ihre Nachricht!</h2>
                        <p class="lead text-white">
                          Strainovic IT<br>
                          Goran Strainovic<br>
                         +41 79 411 71 77<br>
                          <a href='mailto:info@strainovic-it.ch'>info@strainovic-it.ch</a>
                        </p>
                    </div>
                </div>
                <!-- <div class="row row-grid mt-5"> -->
                    <!-- <div class="col-lg-4"> -->
                        <!-- <icon name="ni ni-settings" size="lg" gradient="white" shadow round color="primary"></icon> -->
                        <!-- <h5 class="text-white mt-3">Building tools</h5> -->
                        <!-- <p class="text-white mt-3">Some quick example text to build on the card title and make up the -->
                            <!-- bulk of the card's content.</p> -->
                    <!-- </div> -->
                    <!-- <div class="col-lg-4"> -->
                        <!-- <icon name="ni ni-ruler-pencil" size="lg" gradient="white" shadow round color="primary"></icon> -->
                        <!-- <h5 class="text-white mt-3">Grow your market</h5> -->
                        <!-- <p class="text-white mt-3">Some quick example text to build on the card title and make up the -->
                            <!-- bulk of the card's content.</p> -->
                    <!-- </div> -->
                    <!-- <div class="col-lg-4"> -->
                        <!-- <icon name="ni ni-atom" size="lg" gradient="white" shadow round color="primary"></icon> -->
                        <!-- <h5 class="text-white mt-3">Launch time</h5> -->
                        <!-- <p class="text-white mt-3">Some quick example text to build on the card title and make up the -->
                            <!-- bulk of the card's content.</p> -->
                    <!-- </div> -->
                <!-- </div> -->
            </div>
        </section>
        <section class="section section-lg pt-lg-0 section-contact-us">
            <div class="container">
                <div class="row mt--300">
                    <div class="col-lg-8">
                        <card gradient="secondary" shadow body-classes="p-lg-5">
                            <!-- <h4 class="mb-1">Want to work with us?</h4> -->
                            <!-- <p class="mt-0">Your project is very important to us.</p> -->
                            <base-input class=""
                                        alternative
                                        placeholder="Vorname">
                                        <!-- addon-left-icon="ni ni-user-run"> -->
                            </base-input>
                            <base-input class=""
                                        alternative
                                        placeholder="Nachname">
                                        <!-- addon-left-icon="ni ni-user-run"> -->
                            </base-input>
                            <base-input alternative
                                        placeholder="E-Mail Adresse"
                                        addon-left-icon="ni ni-email-83">
                            </base-input>
                            <base-input class="mb-4">
                                    <textarea class="form-control form-control-alternative" name="name" rows="4"
                                              cols="80" placeholder="Ihre Nachricht"></textarea>
                            </base-input>
                            <base-button type="default" round block size="lg">
                                Senden
                            </base-button>
                        </card>
                    </div>
                </div>
            </div>
        </section>
        <section class="section section-lg">
            <div class="container">
                <div class="row">
                    <div class="col-md-6">
                        <div class="pr-md-6">
                           <h2 class="display-5">Kommen Sie auf ein Beratungsgespräch vorbei</h2>
                           <p class="lead">
                           Ich freue mich Sie persönlich kennenzulernen.<br>
                           Gerne komme ich für 1chf/km auch zu Ihnen.<br>
                           Vereinbaren Sie noch heute einen Termin.<br>
                           </p>
                        </div>
                   </div>
                </div>
                <div class="row">
                    <div class="col-md-3">
                        <p>
                          <br>
                          Strainovic IT<br>
                          Strainovic Goran<br>
                          Bahnstrasse 9b<br>
                          CH 9323 Steinach<br>
                          Kanton St.Gallen SG<br>
                          +41 79 411 71 77<br>
                          <a href='mailto:info@strainovic-it.ch'>info@strainovic-it.ch</a>
                        </p>
                    </div>
                    <div class="col-md-3 mt-5">
                        <VueFriendlyIframe src="https://www.google.com/maps/embed/v1/place?key=AIzaSyDUUYNFXEhy1raQAPrhYCdSCttMLgMsxls      &q=Strainovic IT" allowfullscreen @load="onLoad" @document-load="onDocumentLoad"></VueFriendlyIframe>
                        <!-- <img src="/argon/img/theme/promo-1.png" class="img-fluid floating"> -->
                    </div>
                 </div>
             </div>
        </section>
      <footer class="footer">
       <div class="container">
            <div class="row row-grid align-items-center my-md">
                <div class="col-lg-6">
                    <h3 class="text-primary font-weight-light mb-2">Vielen Dank für Ihre Unterstützung!</h3>
                    <h4 class="mb-0 font-weight-light">Folgen Sie uns auf einer dieser Plattformen.</h4>
                </div>
                <div class="col-lg-6 text-lg-center btn-wrapper">
                    <a target="_blank" href="https://twitter.com/Strainovic_IT"
                       class="btn btn-neutral btn-icon-only btn-twitter btn-round btn-lg" data-toggle="tooltip"
                       title="Folge uns auf Twitter">
                        <i class="fa fa-twitter"></i>
                    </a>
                    <a target="_blank" href="https://www.facebook.com/StrainovicIT/"
                       class="btn btn-neutral btn-icon-only btn-facebook btn-round btn-lg" data-toggle="tooltip"
                       title="Like uns auf Facebook">
                        <i class="fa fa-facebook-square"></i>
                    </a>
                    <a target="_blank" href="https://www.instagram.com/strainovic_it/"
                       class="btn btn-neutral btn-icon-only btn-instagram btn-lg btn-round" data-toggle="tooltip"
                       title="Folge uns auf Instagram">
                        <i class="fa fa-instagram"></i>
                    </a>
                    <a target="_blank" href="https://ch.linkedin.com/in/goran-strainovic"
                       class="btn btn-neutral btn-icon-only btn-linkedin btn-round btn-lg" data-toggle="tooltip"
                       title="Folge uns auf LinkedIn">
                        <i class="fa fa-linkedin"></i>
                    </a>
                       <a target="_blank" href="https://github.com/gstrainovic"
                       class="btn btn-neutral btn-icon-only btn-github btn-round btn-lg" data-toggle="tooltip"
                       title="Spendiere uns einen Stern auf Github">
                        <i class="fa fa-github"></i>
                    </a>
                     <a target="_blank" href="https://www.xing.com/profile/Goran_Strainovic"
                       class="btn btn-neutral btn-icon-only btn-xing btn-round btn-lg" data-toggle="tooltip"
                       title="Folge uns auf Xing">
                        <i class="fa fa-xing"></i>
                    </a>
                </div>
            </div>

          </ul>
            <hr>
            <div class="row">
                <div class="col-md-3">
                  <p>
                    Strainovic IT<br>
                    Bahnstrasse 9b<br>
                    CH 9323 Steinach<br>
                    Kanton St.Gallen SG<br>
                    +41 79 411 71 77<br>
                    <a href='mailto:info@strainovic-it.ch'>info@strainovic-it.ch</a>
                  </p>
                </div>
            <!-- </div> -->
            <!-- <div class="row align-items-center justify-content-md-between"> -->
                <div class="col-md-9">
                    <ul class="nav nav-footer justify-content-end">
                        <li class="nav-item">
                            <nuxt-link :to="{name: 'argon-demo-landing'}" class="nav-link">Kontaktformular</nuxt-link>
                            <!-- <a href="https://www.creative-tim.com" class="nav-link" target="_blank">Creative Tim</a> -->
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
import VueFriendlyIframe from 'vue-friendly-iframe';

export default {
  components: {
    BaseNav,
    CloseButton,
    BaseDropdown,
    headroom,
    VueFriendlyIframe
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
