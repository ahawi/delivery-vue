<template>
  <footer class="footer container">
    <div class="footer__inner">
      <router-link to="/" class="footer__logo">
        <img
          class="logo"
          src="../assets/images/icons/logo.svg"
          alt="Delivery Food"
          width="100"
          height="36"
          loading="lazy"
        />
      </router-link>
      <nav class="footer__menu">
        <ul class="footer__menu-list">
          <li class="footer__menu-item">
            <a href="./goods.html" class="footer__menu-link">Ресторанам</a>
          </li>
          <li class="footer__menu-item">
            <a href="./goods.html" class="footer__menu-link">Курьерам</a>
          </li>
          <li class="footer__menu-item">
            <a href="./goods.html" class="footer__menu-link">Пресс-центр</a>
          </li>
          <li class="footer__menu-item">
            <a href="./goods.html" class="footer__menu-link">Контакты</a>
          </li>
        </ul>
      </nav>
      <div class="footer__soc1als">
        <ul class="footer__soc1als-list">
          <li class="footer__soc1als-item">
            <a href="#" class="footer__soc1als-link">
              <span class="visually-hidden">Instagram</span>
              <svg
                width="26"
                height="26"
                viewBox="0 0 26 26"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M18.1353 0.314819H8.76025C4.44619 0.314819 0.947754 3.81326 0.947754 8.12732V17.5023C0.947754 21.8164 4.44619 25.3148 8.76025 25.3148H18.1353C22.4493 25.3148 25.9478 21.8164 25.9478 17.5023V8.12732C25.9478 3.81326 22.4493 0.314819 18.1353 0.314819ZM23.604 17.5023C23.604 20.5179 21.1509 22.9711 18.1353 22.9711H8.76025C5.74463 22.9711 3.2915 20.5179 3.2915 17.5023V8.12732C3.2915 5.11169 5.74463 2.65857 8.76025 2.65857H18.1353C21.1509 2.65857 23.604 5.11169 23.604 8.12732V17.5023Z"
                  fill="url(#paint0_linear_243_55)"
                />
                <path
                  d="M13.4478 6.56482C9.99619 6.56482 7.19775 9.36326 7.19775 12.8148C7.19775 16.2664 9.99619 19.0648 13.4478 19.0648C16.8993 19.0648 19.6978 16.2664 19.6978 12.8148C19.6978 9.36326 16.8993 6.56482 13.4478 6.56482ZM13.4478 16.7211C11.2946 16.7211 9.5415 14.9679 9.5415 12.8148C9.5415 10.6601 11.2946 8.90857 13.4478 8.90857C15.6009 8.90857 17.354 10.6601 17.354 12.8148C17.354 14.9679 15.6009 16.7211 13.4478 16.7211Z"
                  fill="url(#paint1_linear_243_55)"
                />
                <path
                  d="M20.1666 6.92892C20.6265 6.92892 20.9994 6.55606 20.9994 6.09611C20.9994 5.63617 20.6265 5.26331 20.1666 5.26331C19.7066 5.26331 19.3337 5.63617 19.3337 6.09611C19.3337 6.55606 19.7066 6.92892 20.1666 6.92892Z"
                  fill="url(#paint2_linear_243_55)"
                />
                <defs>
                  <linearGradient
                    id="paint0_linear_243_55"
                    x1="3.23627"
                    y1="23.0265"
                    x2="23.6592"
                    y2="2.60318"
                    gradientUnits="userSpaceOnUse"
                  >
                    <stop stop-color="#FFC107" />
                    <stop offset="0.507" stop-color="#F44336" />
                    <stop offset="0.99" stop-color="#9C27B0" />
                  </linearGradient>
                  <linearGradient
                    id="paint1_linear_243_55"
                    x1="9.02846"
                    y1="17.2341"
                    x2="17.8671"
                    y2="8.39552"
                    gradientUnits="userSpaceOnUse"
                  >
                    <stop stop-color="#FFC107" />
                    <stop offset="0.507" stop-color="#F44336" />
                    <stop offset="0.99" stop-color="#9C27B0" />
                  </linearGradient>
                  <linearGradient
                    id="paint2_linear_243_55"
                    x1="19.5777"
                    y1="6.6851"
                    x2="20.7554"
                    y2="5.50728"
                    gradientUnits="userSpaceOnUse"
                  >
                    <stop stop-color="#FFC107" />
                    <stop offset="0.507" stop-color="#F44336" />
                    <stop offset="0.99" stop-color="#9C27B0" />
                  </linearGradient>
                </defs>
              </svg>
            </a>
          </li>
          <li class="footer__soc1als-item">
            <a href="#" class="footer__soc1als-link">
              <span class="visually-hidden">Facebook</span>
              <svg
                width="25.000000"
                height="25.000000"
                viewBox="0 0 25 25"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
              >
                <path
                  d="M21.87 0L3.12 0C1.4 0 0 1.4 0 3.12L0 21.87C0 23.59 1.4 25 3.12 25L21.87 25C23.59 25 25 23.59 25 21.87L25 3.12C25 1.4 23.59 0 21.87 0Z"
                  fill="#1976D2"
                  fill-opacity="1.000000"
                  fill-rule="nonzero"
                />
                <path
                  d="M21.09 12.5L17.18 12.5L17.18 9.37C17.18 8.51 17.88 8.59 18.75 8.59L20.31 8.59L20.31 4.68L17.18 4.68C14.59 4.68 12.5 6.78 12.5 9.37L12.5 12.5L9.37 12.5L9.37 16.4L12.5 16.4L12.5 25L17.18 25L17.18 16.4L19.53 16.4L21.09 12.5Z"
                  fill="#FAFAFA"
                  fill-opacity="1.000000"
                  fill-rule="nonzero"
                />
              </svg>
            </a>
          </li>
          <li class="footer__soc1als-item">
            <a href="#" class="footer__soc1als-link">
              <span class="visually-hidden">VK</span>
              <svg
                width="35.052307"
                height="20.000000"
                viewBox="0 0 35.0523 20"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
              >
                <path
                  id="Vector"
                  d="M17.15 19.91L19.24 19.91C19.24 19.91 19.87 19.84 20.2 19.49C20.49 19.17 20.48 18.57 20.48 18.57C20.48 18.57 20.44 15.76 21.75 15.35C23.03 14.94 24.69 18.06 26.44 19.27C27.76 20.18 28.76 19.98 28.76 19.98L33.45 19.91C33.45 19.91 35.9 19.76 34.73 17.83C34.64 17.68 34.06 16.41 31.25 13.81C28.32 11.08 28.71 11.52 32.25 6.81C34.4 3.94 35.26 2.19 34.99 1.44C34.74 0.72 33.15 0.91 33.15 0.91L27.89 0.94C27.89 0.94 27.5 0.89 27.2 1.06C26.92 1.24 26.74 1.63 26.74 1.63C26.74 1.63 25.91 3.85 24.79 5.74C22.45 9.73 21.51 9.94 21.12 9.69C20.23 9.11 20.45 7.37 20.45 6.13C20.45 2.27 21.04 0.66 19.31 0.25C18.74 0.11 18.32 0.01 16.85 0C14.97 -0.02 13.38 0.01 12.48 0.45C11.88 0.74 11.42 1.4 11.7 1.43C12.05 1.48 12.84 1.64 13.26 2.21C13.8 2.95 13.78 4.6 13.78 4.6C13.78 4.6 14.09 9.15 13.05 9.71C12.34 10.1 11.36 9.31 9.27 5.69C8.2 3.84 7.39 1.79 7.39 1.79C7.39 1.79 7.23 1.41 6.96 1.21C6.62 0.96 6.15 0.88 6.15 0.88L1.14 0.91C1.14 0.91 0.39 0.93 0.11 1.26C-0.14 1.55 0.09 2.15 0.09 2.15C0.09 2.15 4.01 11.32 8.45 15.95C12.52 20.19 17.15 19.91 17.15 19.91Z"
                  fill="#1E88E5"
                  fill-opacity="1.000000"
                  fill-rule="nonzero"
                />
              </svg>
            </a>
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style scoped>
.footer {
  padding-block: 60px;
  background-color: var(--color-light);
}

.footer__inner {
  display: flex;
  justify-content: space-between;
  align-items: center;
  column-gap: 36px;
}

.footer__menu {
  flex: 1;
}

.footer__logo {
  flex-shrink: 0;
}

.footer__menu-list {
  display: flex;
  column-gap: 15px;
}

.footer__menu-link {
  color: var(--color-gray-dark);
  font-size: 18px;
  white-space: nowrap;
}

.footer__menu-link:hover {
  opacity: 0.7;
}

.footer__soc1als {
  display: flex;
}

.footer__soc1als-list {
  display: flex;
  column-gap: 21px;
  align-items: center;
}

.footer__soc1als-link:hover {
  opacity: 0.7;
}

@media (max-width: 950px) {
  .footer {
    padding-block: 40px;
  }

  .footer__inner {
    column-gap: 10px;
  }

  .footer__menu-list {
    justify-content: end;
    row-gap: 15px;
  }

  .footer__menu-link {
    font-size: 16px;
  }

  .footer__soc1als-list {
    column-gap: 10px;
  }
}

@media (max-width: 625px) {
  .footer__inner {
    column-gap: 20px;
  }

  .footer__menu-list {
    flex-direction: column;
    align-items: end;
  }

  .footer__soc1als {
    justify-content: end;
  }

  .footer__soc1als-list {
    flex-direction: column;
    row-gap: 15px;
  }

  .logo {
    scale: 2;
    padding-left: 30px;
  }
}

@media (max-width: 450px) {
  .footer {
    padding-block: 20px;
  }

  .footer__inner {
    row-gap: 10px;
  }

  .footer__menu-list {
    gap: 10px;
  }

  .footer__soc1als-list {
    display: flex;
    align-items: end;
    justify-content: end;
  }
}
</style>
