                    </div>
                </li>
                 <li class="nav-item dropdown">
                    <a href="#" class="nav-link" data-toggle="dropdown" role="button">
                    </a>
                    <div class="dropdown-menu">
                   </div>
                </li>
                  <li class="nav-item dropdown">
                    <a href="#" class="nav-link" data-toggle="dropdown" role="button">
                    </a>
                    <div class="dropdown-menu">
                   </div>
                </li>
            </ul>
       </base-nav>
    </header>
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
                    <a target="_blank" href="https://github.com/gstrainovic"
                       class="btn btn-neutral btn-icon-only btn-github btn-round btn-lg" data-toggle="tooltip"
                       title="Spendiere mir einen Stern auf Github">
                        <i class="fa fa-github"></i>
                    </a>
                      <a target="_blank" href="https://ch.linkedin.com/in/goran-strainovic"
                       class="btn btn-neutral btn-icon-only btn-linkedin btn-round btn-lg" data-toggle="tooltip"
                       title="Folge mir auf LinkedIn">
                        <i class="fa fa-linkedin"></i>
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
import CloseButton from "~/components/argon/CloseButton";

export default {
  components: {
    BaseNav,
    CloseButton
  }
};
</script>

<style>

</style>
