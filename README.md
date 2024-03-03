# alfa-web-portofolio
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Dev Portofolio</title>
    <style>
      /* Internal CSS */

      section {
        padding-top: 5rem;
      }

      /* jumbotron section Start */
      .jumbotron {
        padding-top: 6rem;
        background-color: #e2edff;
      }
      /* jumbotron section End */

      /* projects section  start */
      #project {
        background-color: #e2edff;
      }
      /* projects section  start */

      /* Study Section Start */
      .study {
        position: relative;
        padding: 45px 0 15px 0;
      }

      .study .timeline {
        position: relative;
      }

      .study .timeline::after {
        content: "";
        position: absolute;
        width: 2px;
        background: #1d5abc;
        top: 0;
        bottom: 0;
        left: 50%;
        margin-left: -1px;
      }

      .study .timeline .timeline-item {
        position: relative;
        width: 50%;
        margin-bottom: 30px;
      }

      .study .timeline .timeline-item.left {
        left: 0;
        padding-right: 30px;
      }

      .study .timeline .timeline-item.right {
        left: 50%;
        padding-left: 30px;
      }

      .study .timeline .timeline-item::after {
        content: "";
        position: absolute;
        width: 16px;
        height: 16px;
        top: 48px;
        right: -8px;
        background: #ffffff;
        border: 2px solid #1d5abc;
        border-radius: 16px;
        z-index: 1;
      }

      .study .timeline .timeline-item.right::after {
        left: -8px;
      }

      .study .timeline .timeline-tanggal {
        position: absolute;
        width: 100%;
        top: 44px;
        font-size: 16px;
        font-weight: 600;
        color: #1d5abc;
        letter-spacing: 1px;
        z-index: 1;
      }

      .study .timeline .timeline-item.left .timeline-tanggal {
        text-align: left;
        left: calc(100% + 55px);
      }

      .study .timeline .timeline-item.right .timeline-tanggal {
        text-align: right;
        right: calc(100% + 55px);
      }

      .study .timeline .timeline-text {
        padding: 30px;
        background: #e2edff;
        position: relative;
        border-radius: 10px;
        box-shadow: 0 0 60px rgba(0, 0, 0, 0.08);
      }

      .study .timeline .timeline-text h2 {
        margin: 0 0 5px 0;
        font-size: 22px;
        font-weight: 600;
      }

      .study .timeline .timeline-text h4 {
        margin: 0 0 10px 0;
        font-size: 16px;
        font-style: italic;
        font-weight: 400;
      }

      .study .timeline .timeline-text p {
        font-size: 16px;
      }

      /* tampilan layar kecil/mobile study section */
      @media (max-width: 767.98px) {
        .study .timeline::after {
          left: 8px;
        }

        .study .timeline .timeline-item {
          width: 100%;
          padding-left: 38px;
        }

        .study .timeline .timeline-item.left {
          padding-right: 0;
        }

        .study .timeline .timeline-item.right {
          left: 0%;
          padding-left: 38px;
        }

        .study .timeline .timeline-item.left::after,
        .study .timeline .timeline-item.right::after {
          left: 0;
        }

        .study .timeline .timeline-item.left::before,
        .study .timeline .timeline-item.right::before {
          left: 18px;
          border-color: transparent #dddddd transparent transparent;
        }

        .study .timeline .timeline-item.left .timeline-tanggal,
        .study .timeline .timeline-item.right .timeline-tanggal {
          position: relative;
          top: 0;
          right: auto;
          left: 0;
          text-align: left;
          margin-bottom: 10px;
        }
      }
      /* Study Section End */

      /* contact section  start */
      #contact {
        background-color: #e2edff;
      }
      /* contact section  end */

      /*  Footer Start */
      .footer {
        position: relative;
        margin-top: 40px;
      }

      .footer .container-fluid {
        padding: 20px 0 0 0;
      }

      .footer .footer-info {
        position: relative;
        width: 100%;
        text-align: center;
      }

      .footer .footer-info h2 {
        margin-bottom: 20px;
        font-size: 25px;
        font-weight: 700;
        color: #ffffff;
      }

      .footer .footer-info h3 {
        margin-bottom: 25px;
        font-size: 18px;
        font-weight: 600;
        color: #ffffff;
      }

      .footer .footer-menu {
        width: 100%;
        display: flex;
        justify-content: center;
      }

      .footer .footer-menu p {
        color: #ffffff;
        font-size: 22px;
        font-weight: 600;
        line-height: 20px;
        padding: 0 15px;
        border-right: 1px solid #ffffff;
      }

      .footer .footer-menu p:last-child {
        border: none;
      }

      .footer .footer-social a i {
        margin-right: 15px;
        font-size: 20px;
        color: #ffffff;
        transition: 0.3s;
      }

      .footer .copyright {
        position: relative;
        text-align: center;
        padding-bottom: 25px;
      }

      .footer .copyright::before {
        position: absolute;
        content: "";
        width: 50%;
        height: 1px;
        top: 0;
        left: 25%;
        background: rgba(256, 256, 256, 0.2);
      }

      .footer .copyright p {
        margin: 0;
        color: #ffffff;
      }

      .footer .copyright .col-md-6:last-child p {
        text-align: right;
      }

      .footer .copyright p a {
        color: #ffffff;
        font-weight: 600;
      }

      .footer .copyright p a:hover {
        color: #414141;
      }

      /* tampilan layar kecil/mobile footer */
      @media (max-width: 575.98px) {
        .footer .footer-info h2 {
          margin-bottom: 20px;
          font-size: 20px;
          font-weight: 600;
        }

        .footer .footer-info h3 {
          margin-bottom: 20px;
          font-size: 16px;
        }

        .footer .footer-menu p {
          font-size: 16px;
          line-height: 16px;
          padding: 0 5px;
        }
      }
      /*  Footer End */
    </style>
  </head>
  <body id="home">
    <!DOCTYPE html>
    <html lang="en">
      <head>
        <meta charset="utf-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1" />
        <title>Portofolio Alfa</title>
        <link
          href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
          rel="stylesheet"
          integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH"
          crossorigin="anonymous"
        />
      </head>
      <body>
        <!-- Navbar Start -->
        <nav
          class="navbar navbar-expand-lg navbar-dark bg-primary shadow fixed-top"
        >
          <div class="container">
            <a class="navbar-brand" href="#">alfa\rhb</a>
            <button
              class="navbar-toggler"
              type="button"
              data-bs-toggle="collapse"
              data-bs-target="#navbarNav"
              aria-controls="navbarNav"
              aria-expanded="false"
              aria-label="Toggle navigation"
            >
              <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
              <ul class="navbar-nav ms-auto">
                <li class="nav-item">
                  <a class="nav-link text-light" href="#home">Home</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link text-light" href="#about">About</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link text-light" href="#project">Project</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link text-light" href="#study">Study</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link text-light" href="#contact">Contact</a>
                </li>
              </ul>
            </div>
          </div>
        </nav>
        <!-- Navbar End -->

        <!-- Jumbotron Start -->
        <section class="jumbotron text-center">
          <img
            src="gambar/den.png"
            alt="Alfaso Rahakbauw"
            width="100px"
            height="100px"
            class="rounded-circle img-thumbnail"
          />
          <h1 class="display-4">Alfaso Rahakbauw</h1>
          <p class="lead">Student | Web Developer</p>
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
            <path
              fill="#fff"
              fill-opacity="1"
              d="M0,160L48,160C96,160,192,160,288,170.7C384,181,480,203,576,176C672,149,768,75,864,53.3C960,32,1056,64,1152,85.3C1248,107,1344,117,1392,122.7L1440,128L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"
            ></path>
          </svg>
        </section>
        <!-- Jumbotron End -->

        <!-- About Start -->
        <section id="about">
          <div class="container mb-5">
            <div class="row text-center mb-3">
              <h2>About</h2>
            </div>
            <div class="row justify-content-center text-center fs-3">
              <div class="col-md-4 fs-5 text-center">
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Iure
                  pariatur laudantium perspiciatis dicta tempore at delectus,
                  vel adipisci beatae consequatur odit quae. Dolore
                  reprehenderit voluptatem similique non omnis neque
                  dignissimos!
                </p>
              </div>
              <div class="col-md-4 fs-5 text-center">
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Iure
                  pariatur laudantium perspiciatis dicta tempore at delectus,
                  vel adipisci beatae consequatur odit quae. Dolore
                  reprehenderit voluptatem similique non omnis neque
                  dignissimos!
                </p>
              </div>
            </div>
          </div>
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
            <path
              fill="#e2edff"
              fill-opacity="1"
              d="M0,128L48,154.7C96,181,192,235,288,218.7C384,203,480,117,576,101.3C672,85,768,139,864,144C960,149,1056,107,1152,101.3C1248,96,1344,128,1392,144L1440,160L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"
            ></path>
          </svg>
        </section>
        <!-- About End -->

        <!-- Project Start -->
        <section id="project">
          <div class="container">
            <div class="row text-center">
              <div class="col mb-3">
                <h2>Projects</h2>
              </div>
            </div>
            <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
              <div class="col">
                <div class="card shadow-sm">
                  <img
                    src="projects/projek landing-page-HtmlCss.png"
                    class="card-img-top"
                    alt="Landing Page"
                  />
                  <div class="card-body">
                    <h5 class="card-title">Landing Page</h5>
                    <p class="card-text">
                      Landing Page rancangan saya sendiri menggunakan HTML & CSS
                    </p>
                  </div>
                </div>
              </div>
              <div class="col">
                <div class="card shadow-sm">
                  <img
                    src="projects/andy-vult-t-WkBEOQngs-unsplash.jpg"
                    class="card-img-top"
                    alt="Foto"
                  />
                  <div class="card-body">
                    <h5 class="card-title">Aestethic Photo</h5>
                    <p class="card-text">
                      hasil potret kamera sony lensa panjang di museum
                    </p>
                  </div>
                </div>
              </div>
              <div class="col">
                <div class="card shadow-sm">
                  <img
                    src="projects/projek-login-form .png"
                    class="card-img-top"
                    alt="Form Login"
                  />
                  <div class="card-body">
                    <h5 class="card-title">Login-Form</h5>
                    <p class="card-text">
                      Responsive login form yang juga saya buat menggunakan HTML
                      & CSS
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </section>
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
          <path
            fill="#e2edff"
            fill-opacity="1"
            d="M0,128L48,154.7C96,181,192,235,288,218.7C384,203,480,117,576,101.3C672,85,768,139,864,144C960,149,1056,107,1152,101.3C1248,96,1344,128,1392,144L1440,160L1440,0L1392,0C1344,0,1248,0,1152,0C1056,0,960,0,864,0C768,0,672,0,576,0C480,0,384,0,288,0C192,0,96,0,48,0L0,0Z"
          ></path>
        </svg>
        <!-- Project End -->

        <!-- Study Start -->
        <section class="study" id="study">
          <div class="container">
            <div class="text-center mb-3">
              <h2>Pendidikan</h2>
            </div>
            <div class="timeline">
              <div class="timeline-item left wow slideInLeft">
                <div class="timeline-text">
                  <div class="timeline-tanggal">2008 - 2014</div>
                  <h2>SD Naskat Mathias 1 Kota Tual</h2>
                  <h4>Jl Dihir no 4, Maluku Tenggara, Tual</h4>
                </div>
              </div>
              <div class="timeline-item right wow slideInRight">
                <div class="timeline-text">
                  <div class="timeline-tanggal">2015 - 2017</div>
                  <h2>SMP Negeri 1 Kota Tual</h2>
                  <h4>Jl Dokter Leimena, Maluku Tenggara, Tual</h4>
                </div>
              </div>
              <div class="timeline-item left wow slideInLeft">
                <div class="timeline-text">
                  <div class="timeline-tanggal">2018 - 2020</div>
                  <h2>SMA Negeri 1 Kota Tual</h2>
                  <h4>Jl Budi Utomo no 4, Maluku Tenggara, Tual</h4>
                </div>
              </div>
              <div class="timeline-item right wow slideInRight">
                <div class="timeline-text">
                  <div class="timeline-tanggal">2021 - Present</div>
                  <h2>Universitas Amikom Yogyakarta</h2>
                  <h4>Jl Condongcatur, Sleman, Yogyakarta</h4>
                </div>
              </div>
            </div>
          </div>
        </section>
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
          <path
            fill="#e2edff"
            fill-opacity="1"
            d="M0,128L48,144C96,160,192,192,288,192C384,192,480,160,576,154.7C672,149,768,171,864,149.3C960,128,1056,64,1152,69.3C1248,75,1344,149,1392,186.7L1440,224L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"
          ></path>
        </svg>
        <!-- Study End -->

        <section id="contact">
          <!-- Contact Start -->
          <div class="container">
            <div class="row">
              <div class="col text-center">
                <h2>Contact</h2>
              </div>
            </div>
            <div class="row justify-content-center">
              <div class="col-md-6">
                <form>
                  <div class="mb-3">
                    <label for="name" class="form-label">Nama Anda</label>
                    <input
                      type="text"
                      class="form-control"
                      id="name"
                      aria-describedby="name"
                    />
                  </div>
                  <div class="mb-3">
                    <label for="email" class="form-label">Email</label>
                    <input
                      type="email"
                      class="form-control"
                      id="email"
                      aria-describedby="email"
                    />
                  </div>
                  <div class="mb-3">
                    <label for="pesan" class="form-label"
                      >Berikan pesan disini</label
                    >
                    <textarea
                      class="form-control"
                      id="pesan"
                      rows="3"
                    ></textarea>
                  </div>
                  <button type="submit" class="btn btn-primary">Kirim</button>
                </form>
              </div>
            </div>
          </div>
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
            <path
              fill="#ffff"
              fill-opacity="1"
              d="M0,160L48,181.3C96,203,192,245,288,245.3C384,245,480,203,576,181.3C672,160,768,160,864,170.7C960,181,1056,203,1152,208C1248,213,1344,203,1392,197.3L1440,192L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"
            ></path>
          </svg>
        </section>
        <!-- Contact End -->

        <!-- Footer -->
        <!-- Footer Start -->
        <footer class="footer wow fadeIn bg-primary shadow">
          <div class="container-fluid">
            <div class="container">
              <div class="footer-info">
                <h2>Alfaso Rahakbauw</h2>
                <h3>Jl Paingan 4, Maguwoharjo, Yogyakarta</h3>
                <div class="footer-menu">
                  <p>0813-4330-5212</p>
                  <p>alfasorahakbauw53@gmail.com</p>
                </div>
              </div>
            </div>
            <div class="container copyright">
              <p>&copy; <a href="#">alfa\rhb</a> | Alfaso Rahakbauw</p>
            </div>
          </div>
        </footer>
        <!-- Footer End -->
        <!-- Footer -->

        <script
          src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"
          integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz"
          crossorigin="anonymous"
        ></script>
      </body>
    </html>
  </body>
</html>
