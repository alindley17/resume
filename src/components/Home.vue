<template>
  <div class="section">
    <div class="container">
      <div class="tile is-ancestor">
        <div class="tile is-vertical is-8">
          <div class="tile">
            <div class="tile is-parent is-vertical">
              <article class="tile is-child card">
                <div class="card-image">
                  <figure class="image is-3by2">
                    <img src="@/assets/headshot_smaller.jpg" alt="Headshot">
                  </figure>
                </div>
                <div class="card-content">
                  <div class="is-size-3 has-text-weight-bold has-text-left">Andrew Lindley</div>
                  <div class="is-size-5 has-text-weight-normal has-text-left">Full-stack Developer</div>
                  <b-icon class="social-media-icon" icon="linkedin" size="is-small" @click.native="redirect('https://www.linkedin.com/in/andrew-lindley-a8075a143/')">
                  </b-icon>
                  <b-icon class="social-media-icon" icon="github" size="is-small" @click.native="redirect('https://github.com/alindley17')">
                  </b-icon>
                  <b-icon class="social-media-icon" icon="twitter" size="is-small" @click.native="redirect('https://twitter.com/drewzle_')">
                  </b-icon>
                </div>
              </article>
              <article class="tile is-child card">
                <div class="card-content">
                  <div class="is-size-5 has-text-weight-bold has-text-left">About Me</div>
                  <div class="is-size-7 has-text-weight-normal has-text-left">Versatile Full-stack Developer with 3+ years of experience designing, developing, and maintaining complex spatial applications and internal data management tools. Builds front-to-back systems including databases, APIs and reactive client-side applications. Specializes in Vue, Node, responsive design and Agile development.</div>
                </div>
              </article>
            </div>
            <div class="tile is-parent">
              <article class="tile is-child card">
                <div class="card-content is-paddingless">
                  <div class="is-size-5 has-text-weight-bold has-text-left custom-padding">Experience</div>
                  <div class="is-size-7 has-text-weight-normal has-text-left custom-padding">
                    <div class="has-text-left has-text-weight-bold">Bright Rain Solutions, Full-stack Developer</div>
                    <div>May '17 - Jun '20</div>
                  </div>
                  <div class="is-size-7 exp-container">

                    <b-collapse animation="slide" :open="true">
                      <div slot="trigger" slot-scope="props" class="card-header card-header-hover" role="button">
                        <p class="card-header-title">
                          Lead development on enterprise-level applications
                        </p>
                        <a class="card-header-icon">
                          <b-icon type="is-dark" :icon="props.open ? 'menu-up' : 'menu-down'">
                          </b-icon>
                        </a>
                      </div>
                      <div class="card-content">
                        <div class="content">
                          <li>Design and develop application layout and tools critical to client operations</li>
                          <li>Design and develop internal dashboard to give client better access to their data</li>
                          <li>Write detailed documentation</li>
                          <li>Test, stage, and deploy application to production</li>
                        </div>
                      </div>
                    </b-collapse>
                    <b-collapse animation="slide" :open="false">
                      <div slot="trigger" slot-scope="props" class="card-header card-header-hover" role="button">
                        <p class="card-header-title">
                          Design and deploy reactive responsive front-end applications with intuitive UI/UX
                        </p>
                        <a class="card-header-icon">
                          <b-icon type="is-dark" :icon="props.open ? 'menu-up' : 'menu-down'">
                          </b-icon>
                        </a>
                      </div>
                      <div class="card-content">
                        <div class="content">
                          <li>Create dynamic applications that manage user security</li>
                        </div>
                      </div>
                    </b-collapse>
                    <b-collapse animation="slide" :open="false">
                      <div slot="trigger" slot-scope="props" class="card-header card-header-hover" role="button">
                        <p class="card-header-title">
                          Build CRUD APIs that securely manage users and communication with the database
                        </p>
                        <a class="card-header-icon">
                          <b-icon type="is-dark" :icon="props.open ? 'menu-up' : 'menu-down'">
                          </b-icon>
                        </a>
                      </div>
                      <div class="card-content">
                        <div class="content">
                          <li>Implement custom user authentication with encrypted credentials</li>
                        </div>
                      </div>
                    </b-collapse>
                    <div>
                      <div class="card-header card-header-default">
                        <p class="card-header-title">
                          Design data structures and create databases
                        </p>
                      </div>
                    </div>
                    <div>
                      <div class="card-header card-header-default">
                        <p class="card-header-title">
                          Communicate directly with clients to incorporate feedback and plan future milestones
                        </p>
                      </div>
                    </div>
                    <div>
                      <div class="card-header card-header-default">
                        <p class="card-header-title">
                          Work with a small team to complete deliverables on time
                        </p>
                      </div>
                    </div>
                    <div>
                      <div class="card-header card-header-default">
                        <p class="card-header-title">
                          Engage with prospective clients to procure new contracts
                        </p>
                      </div>
                    </div>
                  </div>
                </div>
              </article>
            </div>
          </div>

          <div class="tile is-parent">
            <article class="tile is-child card">
              <div class="card-content">
                <div class="is-size-5 margin-bot">
                  <b-field grouped group-multiline>
                    <span class="margin-right has-text-weight-bold">Skills</span>
                    <b-taglist>
                      <b-tag rounded class="info-light">Web</b-tag>
                      <b-tag rounded class="success-light">API</b-tag>
                      <b-tag rounded class="warning-light">Server</b-tag>
                      <b-tag rounded>Other</b-tag>
                    </b-taglist>
                  </b-field>
                </div>

                <div class="is-size-7 has-text-weight-normal">
                  <b-field grouped group-multiline>
                    <span class="has-text-weight-bold">Proficient:</span>
                    <b-taglist>
                      <b-tag rounded class="info-light">Javascript</b-tag>
                      <b-tag rounded class="info-light">Vue</b-tag>
                      <b-tag rounded class="info-light">jQuery</b-tag>
                      <b-tag rounded class="info-light">HTML 5</b-tag>
                      <b-tag rounded class="info-light">CSS3</b-tag>
                      <b-tag rounded class="info-light">SCSS</b-tag>
                      <b-tag rounded class="info-light">ArcGIS JSAPI</b-tag>
                      <b-tag rounded class="info-light">Turf.js</b-tag>
                      <b-tag rounded class="info-light">REST</b-tag>
                      <b-tag rounded class="info-light">AJAX</b-tag>
                      <b-tag rounded class="success-light">Node</b-tag>
                      <b-tag rounded class="success-light">Knex</b-tag>
                      <b-tag rounded class="success-light">Objection.js</b-tag>
                      <b-tag rounded class="warning-light">PostgreSQL</b-tag>
                      <b-tag rounded>Git</b-tag>
                      <b-tag rounded>Digital Ocean</b-tag>
                    </b-taglist>
                  </b-field>
                </div>
                <br>

                <div class="is-size-7 has-text-weight-normal">
                  <b-field grouped group-multiline>
                    <span class="has-text-weight-bold">Intermediate:</span>
                    <b-taglist>
                      <b-tag rounded class="info-light">Webpack</b-tag>
                      <b-tag rounded class="info-light">OpenLayers</b-tag>
                      <b-tag rounded class="info-light">Leaflet</b-tag>
                      <b-tag rounded class="info-light">MapboxGL</b-tag>
                      <b-tag rounded class="info-light">D3</b-tag>
                      <b-tag rounded class="info-light">Markup</b-tag>
                      <b-tag rounded class="success-light">Express</b-tag>
                      <b-tag rounded class="success-light">Passport.js</b-tag>
                      <b-tag rounded class="success-light">SQL</b-tag>
                      <b-tag rounded class="warning-light">SQL Server</b-tag>
                      <b-tag rounded class="warning-light">Linux</b-tag>
                      <b-tag rounded class="warning-light">NginX</b-tag>
                      <b-tag rounded class="warning-light">pm2</b-tag>
                    </b-taglist>
                  </b-field>
                </div>
                <br>

                <div class="is-size-7 has-text-weight-normal">
                  <b-field grouped group-multiline>
                    <span class="has-text-weight-bold">Exposure:</span>
                    <b-taglist>
                      <b-tag rounded class="info-light">React</b-tag>
                      <b-tag rounded class="info-light">Typescript</b-tag>
                      <b-tag rounded class="info-light">Three.js</b-tag>
                      <b-tag rounded class="info-light">Cesium</b-tag>
                      <b-tag rounded class="success-light">Python</b-tag>
                      <b-tag rounded>Nightwatch</b-tag>
                      <b-tag rounded>Selenium</b-tag>
                    </b-taglist>
                  </b-field>
                </div>

              </div>
            </article>
          </div>
        </div>
        <div class="tile is-parent">
          <article class="tile is-child card">


            <div class="card-content">
              <div class="is-size-5 has-text-weight-bold has-text-left">Projects</div>

              <!-- this resume -->
              <article class="media">
                <div class="media-content project-item" @click="redirect('https://github.com/alindley17/resume')">
                  <div class="content is-size-7">
                    <p>
                      <strong>This Resume</strong>
                      <br>
                      Click here to see the github repo where you can download a PDF of this resume
                      <br>
                      <b-taglist>
                        <b-tag rounded class="info-light">Vue</b-tag>
                        <b-tag rounded class="info-light">Webpack</b-tag>
                        <b-tag rounded class="warning-light">Linux</b-tag>
                      </b-taglist>
                    </p>
                  </div>
                </div>
              </article>

              <!-- codepen webmap -->
              <article class="media">
                <div class="media-content project-item" @click="redirect('https://codepen.io/alindley17/pen/VXbLLe')">
                  <div class="content is-size-7">
                    <p>
                      <strong>10 Minute 3D Web Map</strong>
                      <br>
                      A quick demo I put together for a presentation I gave at the Northern Colorado Geo-meetup in March of 2017
                      <br>
                      <b-taglist>
                        <b-tag rounded class="info-light">Codepen</b-tag>
                        <b-tag rounded class="info-light">ArcGIS JSAPI</b-tag>
                      </b-taglist>
                    </p>
                  </div>
                </div>
              </article>

              <!-- map our borders -->
              <article class="media">
                <div class="media-content project-item" @click="redirect('https://mapourborders.com')">
                  <div class="content is-size-7">
                    <p>
                      <strong>Map Our Borders</strong>
                      <br>
                      A mapplication for crowdsourcing place names, built by Bright Rain Solutions
                      <br>
                      <b-taglist>
                        <b-tag rounded class="info-light">Vue</b-tag>
                        <b-tag rounded class="info-light">Webpack</b-tag>
                        <b-tag rounded class="info-light">Leaflet</b-tag>
                        <b-tag rounded class="info-light">H3</b-tag>
                        <b-tag rounded class="success-light">Node</b-tag>
                        <b-tag rounded class="success-light">Knex</b-tag>
                        <b-tag rounded class="success-light">Objection</b-tag>
                        <b-tag rounded class="warning-light">Postgres</b-tag>
                        <b-tag rounded class="warning-light">Linux</b-tag>
                      </b-taglist>
                    </p>
                  </div>
                </div>
              </article>

              <!-- csu trees -->
              <article class="media">
                <div class="media-content project-item"  @click="redirect('https://csutrees.org')">
                  <div class="content is-size-7">
                    <p>
                      <strong>CSU Trees</strong>
                      <br>
                      Another mapplication showing the location of all trees managed by Colorado State University, built by Bright Rain Solutions with the Geospatial Centroid at CSU
                      <br>
                      <b-taglist>
                        <b-tag rounded class="info-light">Vue</b-tag>
                        <b-tag rounded class="info-light">Webpack</b-tag>
                        <b-tag rounded class="info-light">Open Layers</b-tag>
                        <b-tag rounded class="success-light">Node</b-tag>
                        <b-tag rounded class="warning-light">Postgres</b-tag>
                        <b-tag rounded class="warning-light">Linux</b-tag>
                      </b-taglist>
                    </p>
                  </div>
                </div>
              </article>

              <!-- aotw -->

              <article class="media">
                <div class="media-content project-item"  @click="redirect('https://aotw.io')">
                  <div class="content is-size-7">
                    <p>
                      <strong>Album of the Week</strong>
                      <br>
                      A side project I built from the ground-up to serve as a platform for a casual album of the week group with friends. The public page is sparse
                      <br>
                      <b-taglist>
                        <b-tag rounded class="info-light">Vue</b-tag>
                        <b-tag rounded class="info-light">Webpack</b-tag>
                        <b-tag rounded class="success-light">Node</b-tag>
                        <b-tag rounded class="success-light">Knex</b-tag>
                        <b-tag rounded class="success-light">Objection</b-tag>
                        <b-tag rounded class="warning-light">Postgres</b-tag>
                        <b-tag rounded class="warning-light">Linux</b-tag>
                        <b-tag rounded class="warning-light">Digital Ocean</b-tag>
                      </b-taglist>
                    </p>
                  </div>
                </div>
              </article>


            </div>


          </article>
        </div>
      </div>

<!--       <div class="has-text-right is-size-7">
        <span class="is-italic has-text-weight-light">This is a work in progress</span>
      </div> -->

    </div>
  </div>
</template>

<script>
export default {
  name: 'Home',
  data() {
    return {
      msg: 'howdy'
    }
  },
  methods: {
    redirect(url) {
      window.open(url)
    }
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
// #00a4e2
.wrap {
  color: red;
}

.card {
  box-shadow: 0 0.5em 1em -0.125em rgba(10,10,10,.1), 0 0 0 1px rgba(10,10,10,.02) !important;
}

.social-media-icon {
  cursor: pointer;
  transition: all .2s ease-in-out;
}

.social-media-icon:hover {
  color: #e2d400;
  transform: scale(1.25);
}

.exp-container {
  margin-top: 0.5rem;
}

.card-header-hover:hover {
  background-color: hsl(0, 0%, 98%);
}

.card-header-default:hover {
  cursor: default;
}

.project-item {
  padding: 0.25rem;
  cursor: pointer;
}

.project-item:hover {
  background-color: hsl(0, 0%, 98%);
}

.info-light {
  background-color: #eef6fc;
  color: #1d72aa;
}

.success-light {
  background-color: #effaf3;
  color: #257942;
}

.warning-light {
  background-color: #fffbeb;
  color: #947600;
}

.margin-bot {
  margin-bottom: 1rem;
}

.margin-right {
  margin-right: 0.5rem;
}

.custom-padding {
  padding: 1rem;
}

</style>
