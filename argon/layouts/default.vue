<template>
  <div>
    <headroom>
      <header class="header-global">
        <BaseNav class="navbar-main" type="transparent" effect="dark" expand>
          <a slot="brand" class="navbar-brand" href="/#">Strainovic IT</a>
          <div slot="content-header" slot-scope="{ closeMenu }" class="row">
            <div class="col-6 collapse-brand">
              <a href="/#">Strainovic IT</a>
            </div>
            <div class="col-6 collapse-close">
              <CloseButton @click="closeMenu"></CloseButton>
            </div>
          </div>

          <ul
            class="navbar-nav navbar-nav-hover align-items-lg-center ml-lg-auto"
          >
            <!-- <ul class="navbar-nav navbar-nav-hover align-items-lg-center ml-lg-auto"> -->
            <BaseDropdown tag="li" class="nav-item">
              <a
                slot="title"
                href="##"
                class="nav-link"
                data-toggle="dropdown"
                role="button"
              >
                <i class="ni ni-spaceship"></i>
                <span class="nav-link-inner--text">Dienstleistungen</span>
              </a>
              <a href="/#was-wir-tun" class="dropdown-item">Was wir tun</a>
              <a href="/#software-und-apps" class="dropdown-item"
                >Software & Apps</a
              >
              <a href="/#webdesign-und-programmierung" class="dropdown-item"
                >Webdesign & Programmierung</a
              >
              <a href="/#marketing" class="dropdown-item">Marketing</a>
            </BaseDropdown>
            <BaseDropdown tag="li" class="nav-item">
              <a
                slot="title"
                href="/ueber/##"
                class="nav-link"
                data-toggle="dropdown"
                role="button"
              >
                <i class="ni ni-single-02"></i>
                <span class="nav-link-inner--text">Über uns</span>
              </a>
              <a href="/ueber/#strainovic-it" class="dropdown-item"
                >Über Strainovic IT</a
              >
              <a href="/ueber/#goran-strainovic" class="dropdown-item"
                >Über Goran Strainovic</a
              >
            </BaseDropdown>
            <BaseDropdown tag="li" class="nav-item">
              <a
                slot="title"
                href="##"
                class="nav-link"
                data-toggle="dropdown"
                role="button"
              >
                <i class="ni ni-collection"></i>
                <span class="nav-link-inner--text">Portfolio</span>
              </a>
              <a href="/portfolio/#web" class="dropdown-item">Webseiten</a>
              <a href="/portfolio/#diverse-projekte" class="dropdown-item"
                >Diverse Projekte</a
              >
            </BaseDropdown>

            <a class="nav-link" href="#kontakt">
              <i class="ni ni-email-83"></i>
              <span class="nav-link-inner--text">Kontakt</span>
            </a>
          </ul>
        </BaseNav>
      </header>
    </headroom>
    <main>
      <nuxt />
    </main>
    <section id="kontakt" class="section section-shaped my-0 overflow-hidden">
      <div class="shape shape-style-3 bg-gradient-default shape-skew">
        <span></span>
        <span></span>
        <span></span>
        <span></span>
      </div>
      <div class="container pt-lg pb-300">
        <div class="row">
          <div class="col-lg-10">
            <h2 class="display-3 text-white">
              Wir freuen uns auf Ihre Kontaktaufnahme!
            </h2>
            <div class="row">
              <div class="col-md-3 lead text-white">
                <p>
                  <br />
                  Strainovic IT<br />
                  Strainovic Goran<br />
                  Bahnstrasse 9b<br />
                  CH 9323 Steinach<br />
                  Kanton St.Gallen SG<br />
                  +41 79 411 71 77<br />
                  <a href="mailto:info@strainovic-it.ch"
                    >info@strainovic-it.ch</a
                  >
                </p>
              </div>
              <div class="col-md-3 mt-5">
                <VueFriendlyIframe
                  src="https://www.google.com/maps/embed/v1/place?key=AIzaSyDUUYNFXEhy1raQAPrhYCdSCttMLgMsxls      &q=Strainovic IT"
                  allowfullscreen
                  @load="onLoad"
                  @document-load="onDocumentLoad"
                ></VueFriendlyIframe>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="section section-lg pt-lg-0 section-contact-us">
      <div class="container">
        <div class="row mt--300">
          <div class="col-lg-8">
            <card gradient="secondary" shadow body-classes="p-lg-5">
              <!-- <h4 class="mb-1">Want to work with us?</h4> -->
              <!-- <p class="mt-0">Your project is very important to us.</p> -->
              <base-input class="" alternative placeholder="Vorname">
                <!-- addon-left-icon="ni ni-user-run"> -->
              </base-input>
              <base-input class="" alternative placeholder="Nachname">
                <!-- addon-left-icon="ni ni-user-run"> -->
              </base-input>
              <base-input
                alternative
                placeholder="E-Mail Adresse"
                addon-left-icon="ni ni-email-83"
              >
              </base-input>
              <base-input class="mb-4">
                <textarea
                  class="form-control form-control-alternative"
                  name="name"
                  rows="4"
                  cols="80"
                  placeholder="Ihre Nachricht"
                ></textarea>
              </base-input>
              <base-button type="default" round block size="lg">
                Senden
              </base-button>
            </card>
          </div>
        </div>
      </div>
    </section>

    <footer class="footer">
      <div class="container">
        <div class="row row-grid align-items-center my-md">
          <div class="col-lg-6">
            <h3 class="text-primary font-weight-light mb-2">
              Vielen Dank für Ihre Unterstützung!
            </h3>
            <h4 class="mb-0 font-weight-light">
              Folgen Sie uns auf einer dieser Plattformen.
            </h4>
          </div>
          <div class="col-lg-6 text-lg-center btn-wrapper">
            <a
              target="_blank"
              href="https://twitter.com/Strainovic_IT"
              class="btn btn-neutral btn-icon-only btn-twitter btn-round btn-lg"
              data-toggle="tooltip"
              title="Folge uns auf Twitter"
            >
              <i class="fa fa-twitter"></i>
            </a>
            <a
              target="_blank"
              href="https://www.facebook.com/StrainovicIT/"
              class="btn btn-neutral btn-icon-only btn-facebook btn-round btn-lg"
              data-toggle="tooltip"
              title="Like uns auf Facebook"
            >
              <i class="fa fa-facebook-square"></i>
            </a>
            <a
              target="_blank"
              href="https://www.instagram.com/strainovic_it/"
              class="btn btn-neutral btn-icon-only btn-instagram btn-lg btn-round"
              data-toggle="tooltip"
              title="Folge uns auf Instagram"
            >
              <i class="fa fa-instagram"></i>
            </a>
            <a
              target="_blank"
              href="https://ch.linkedin.com/in/goran-strainovic"
              class="btn btn-neutral btn-icon-only btn-linkedin btn-round btn-lg"
              data-toggle="tooltip"
              title="Folge uns auf LinkedIn"
            >
              <i class="fa fa-linkedin"></i>
            </a>
            <a
              target="_blank"
              href="https://github.com/gstrainovic"
              class="btn btn-neutral btn-icon-only btn-github btn-round btn-lg"
              data-toggle="tooltip"
              title="Spendiere uns einen Stern auf Github"
            >
              <i class="fa fa-github"></i>
            </a>
            <a
              target="_blank"
              href="https://www.xing.com/profile/Goran_Strainovic"
              class="btn btn-neutral btn-icon-only btn-xing btn-round btn-lg"
              data-toggle="tooltip"
              title="Folge uns auf Xing"
            >
              <i class="fa fa-xing"></i>
            </a>
          </div>
        </div>
        <hr />
        <div class="row">
          <div class="col-md-3">
            <p>
              Strainovic IT<br />
              Bahnstrasse 9b<br />
              CH 9323 Steinach<br />
              Kanton St.Gallen SG<br />
              +41 79 411 71 77<br />
              <a href="mailto:info@strainovic-it.ch">info@strainovic-it.ch</a>
            </p>
          </div>
          <!-- </div> -->
          <!-- <div class="row align-items-center justify-content-md-between"> -->
          <div class="col-md-9">
            <ul class="nav nav-footer justify-content-end">
              <li class="nav-item">
                <nuxt-link :to="{ name: 'argon-demo-landing' }" class="nav-link"
                  >Kontaktformular</nuxt-link
                >
                <!-- <a href="https://www.creative-tim.com" class="nav-link" target="_blank">Creative Tim</a> -->
              </li>
              <li class="nav-item">
                <a
                  href="https://www.creative-tim.com/presentation"
                  class="nav-link"
                  target="_blank"
                  >About Us</a
                >
              </li>
              <li class="nav-item">
                <a
                  href="http://blog.creative-tim.com"
                  class="nav-link"
                  target="_blank"
                  >Blog</a
                >
              </li>
              <li class="nav-item">
                <a
                  href="https://github.com/creativetimofficial/argon-design-system/blob/master/LICENSE.md"
                  class="nav-link"
                  target="_blank"
                  >MIT License</a
                >
              </li>
            </ul>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import BaseNav from '~/components/argon/BaseNav'
import BaseDropdown from '~/components/argon/BaseDropdown'
import CloseButton from '~/components/argon/CloseButton'
import { headroom } from 'vue-headroom'
import VueFriendlyIframe from 'vue-friendly-iframe'

export default {
  components: {
    BaseNav,
    CloseButton,
    BaseDropdown,
    headroom,
    VueFriendlyIframe
  }
}
</script>
<style>
.headroom--not-top {
  padding-top: 0;
  padding-bottom: 0;
}
@media (min-width: 992px) {
  .navbar-main {
    padding: 0;
  }
}
</style>
