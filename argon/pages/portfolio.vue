<template>
    <div>
        <div class="position-relative">
            <!-- shape Hero -->
            <section class="section-shaped my-0">
                <div class="shape shape-style-1 shape-default shape-skew">
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                </div>
                <div class="container shape-container d-flex">
                    <div class="col px-0">
                        <div class="row">
                            <div class="col-lg-6">
                                <h1 class="display-3  text-white">Unser Portfolio
                                    <span>Webdesign</span>
                                </h1>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
            <!-- 1st Hero Variation -->
        </div>
        <section class="">
            <div class="container">
                <div class="row mb-lg mt-5">
                  <div class="container container-lg">
                      <div class="row">
                          <div class="col-md-6 mb-5 mb-md-0 mt-5">
                              <div class="card card-lift--hover shadow">
                                  <nuxt-link to="/landing" title="Landing Page">
                                      <img v-lazy="'/portfolio-responsive-webdesign/ResponsiveWebDesign-ddp.jpg'" class="card-img-top">
                                  </nuxt-link>
                                  <div class="card-body">
                                     <table class="table">
                                        <tbody>
                                            <tr>
                                              <th>Projekt</th>
                                              <td>Webseite</td>
                                            </tr>
                                            <tr>
                                              <th>Branche</th>
                                              <td>Transportunternehmen</td>
                                            </tr>
                                            <tr>
                                              <th>Firmenort</th>
                                              <td>CH-9403 Goldach SG, Kanton St.Gallen, Schweiz</td>
                                            </tr>
                                            <tr>
                                              <th>Technologie</th>
                                              <td>Grav CMS</td>
                                            </tr>
                                            <tr>
                                              <th>Link</th>
                                              <td><a href="http://ddp-transporte.ch" target="_blank">http://ddp-transporte.ch</a></td>
                                            </tr>
                                        </tbody>
                                    </table>
                                  </div>
                              </div>
                         </div>
                          <div class="col-md-6 mb-5 mb-lg-0 mt-5">
                              <div class="card card-lift--hover shadow border-0">
                                  <nuxt-link :to="{name: 'argon-demo-profile'}" title="Profile Page">
                                      <img v-lazy="'/portfolio-responsive-webdesign/ResponsiveWebDesign-bs.jpg'" class="card-img">
                                  </nuxt-link>
                              </div>
                          </div>
                          <div class="col-md-6 mb-5 mb-lg-0 mt-5">
                              <div class="card card-lift--hover shadow border-0">
                                  <nuxt-link :to="{name: 'argon-demo-profile'}" title="Profile Page">
                                      <img v-lazy="'/portfolio-responsive-webdesign/ResponsiveWebDesign-bs.jpg'" class="card-img">
                                  </nuxt-link>
                              </div>
                          </div>
                          <div class="col-md-6 mb-5 mb-lg-0 mt-5">
                              <div class="card card-lift--hover shadow border-0">
                                  <nuxt-link :to="{name: 'argon-demo-profile'}" title="Profile Page">
                                      <img v-lazy="'/portfolio-responsive-webdesign/ResponsiveWebDesign-bs.jpg'" class="card-img">
                                  </nuxt-link>
                              </div>
                          </div>
                          <div class="col-md-6 mb-5 mb-lg-0 mt-5">
                              <div class="card card-lift--hover shadow border-0">
                                  <nuxt-link :to="{name: 'argon-demo-profile'}" title="Profile Page">
                                      <img v-lazy="'/portfolio-responsive-webdesign/ResponsiveWebDesign-bs.jpg'" class="card-img">
                                  </nuxt-link>
                              </div>
                          </div>
                         </div>
                  </div>
              </div>
            </div>
        </section>
      </div>
    </div>
</template>

<script>

export default {
  name: "home",
  layout: 'default',
  components: {
  }
};
</script>

<style>
.section-shaped .shape.shape-skew + .shape-container {
    padding-top: 14rem;
    padding-bottom: 15rem;
}
</style>
