<style>
  .dock {
    position: absolute;
    bottom: 0px;
    text-align: center;
    display: flex;
    justify-content: center;
    width: 100%;
    left: 0;
  }
  .logo {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
  .logo img {
    max-width: 200px;
  }
  span {
    position: absolute;
    left: 0;
    bottom: 0px;
    width: 100%;
    height: 100px;
    display: block;
    opacity: 0.2;
  }
  .dock-nav ul {
    display: flex;
    align-items: center;
    justify-content: center;
    min-width: 300px;
    padding: 20px;
    position: relative;
  }
  .dock-nav ul li {
    list-style-type: none;
    display: inline-block;
    padding: 0 10px;
    position: relative;
    transition: all 0.3s linear;
    cursor: pointer;
  }
  .dock-nav ul li img {
    width: 50px;
    -webkit-transition: -webkit-transform 0.3s
      cubic-bezier(0.68, -0.55, 0.265, 1.55);
    transition: -webkit-transform 0.3s cubic-bezier(0.68, -0.55, 0.265, 1.55);
    transition: transform 0.3s cubic-bezier(0.68, -0.55, 0.265, 1.55);
    transition: transform 0.3s cubic-bezier(0.68, -0.55, 0.265, 1.55),
      -webkit-transform 0.3s cubic-bezier(0.68, -0.55, 0.265, 1.55);
    -webkit-box-reflect: below 8px -webkit-gradient(linear, right top, right
          bottom, from(transparent), to(rgba(255, 255, 255, 0.4)));
  }
  .dock-nav ul li:hover img {
    transform: translateY(-15px) scale(1.2);
  }
  .dock-nav ul li.other img {
    transform: translateY(-5px);
  }
</style>

<main>
  <!-- Dock -->
  <div class="dock">
    <!-- Nav Background -->
    <span>
      <img
        src="https://image.ibb.co/mHAnwK/nav.png"
        class="img-fluid"
        alt="nav" />
    </span>
    <!-- Dock Nav -->
    <div class="dock-nav">
      <ul>
        <li>
          <img
            src="http://icons.iconarchive.com/icons/johanchalibert/mac-osx-yosemite/1024/finder-icon.png"
            class="img-fluid"
            alt="mac"
             />
        </li>
        <li>
          <img
            src="http://www.macosicongallery.com/icons/squash-2017-09-06/128.png"
            class="img-fluid"
            alt="mac" />
        </li>
        <li>
          <img
            src="http://www.macosicongallery.com/icons/screenflow-7-2017-08-17/128.png"
            class="img-fluid"
            alt="mac" />
        </li>
        <li>
          <img
            src="http://www.macosicongallery.com/icons/snapheal-fix-your-photos-2017-10-23/512.png"
            class="img-fluid"
            alt="mac" />
        </li>
        <li>
          <img
            src="http://www.macosicongallery.com/icons/twitterrific-5-for-twitter-2017-10-23/128.png"
            class="img-fluid"
            alt="mac" />
        </li>
        <li>
          <img
            src="http://www.macosicongallery.com/icons/linea-link-2017-07-28/128.png"
            class="img-fluid"
            alt="mac" />
        </li>
        <li>
          <img
            src="http://www.macosicongallery.com/icons/rapidweaver-7-2017-05-19/128.png"
            class="img-fluid"
            alt="mac" />
        </li>
        <li>
          <img
            src="http://www.macosicongallery.com/icons/owly-display-sleep-prevention-2017-03-20/128.png"
            class="img-fluid"
            alt="mac" />
        </li>
      </ul>
    </div>
  </div>
</main>
