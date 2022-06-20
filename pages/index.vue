<template>
  <div class='container'>
    <div class='row'>
      <!--Left Menu block-->
      <div class='col-lg-3 col-md-1 col-2'>
        <nav>
          <a href="#">
            <i class="fab fa-twitter fa-2x"></i>
          </a>
          <ul class="nav flex-column">
            <li class="nav-item">
              <a class="nav-link active" href="#">
                <i class="fas fa-house-damage"></i>
                <span class="menu-text">Home</span>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <i class="fab fa-slack-hash"></i>
                <span class="menu-text">Explore</span>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <i class="far fa-bell"></i>
                <span class="menu-text">Notifications</span>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <i class="far fa-envelope"></i>
                <span class="menu-text">Messages</span>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <i class="far fa-bookmark"></i>
                <span class="menu-text">Bookmarks</span>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <i class="far fa-list-alt"></i>
                <span class="menu-text">Lists</span>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <i class="far fa-user-circle"></i>
                <span class="menu-text">Profile</span>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <i class="fas fa-ellipsis-h"></i>
                <span class="menu-text">More</span>
              </a>
            </li>
            <li class="nav-item mobile-post">
              <a class="nav-link2" href="#">
                <i class="far fa-edit"></i>
              </a>
            </li>
          </ul>
          <button type="button" class="btn btn-primary btn-sm tweeterBtn">Tweet</button>
        </nav>
      </div>
      <!--middle block-->
      <div class='col-lg-6 col-md-11 col-10'>
        <main>
          <div class="first-part">
            <div>
              <a class="home">Beranda</a>
            </div>
            <div>
              <i class="far fa-star"></i>
            </div>
          </div>
          <div class="whats-happening">
            <form>
              <div class="post-blocks">
                <div class="post-profile">
                  <img src="/img_avatar2.png" class="avatar" alt="Avatar">
                </div>
                <textarea class="post-form" placeholder="Apa yang sedang terjadi?"></textarea>
              </div>
              <div class="post-icons">
                <div class="first-post-icons">
                  <i class="fas fa-image"></i>
                  <i class="fas fa-gift"></i>
                  <i class="fas fa-signal"></i>
                  <i class="fas fa-smile"></i>
                </div>
                <div class="second-post-icons">
                  <i class="far fa-circle"></i>
                  <i class="fas fa-plus-circle"></i>
                  <button type="button" class="btn btn-primary btn-sm tweeterBtn">Tweet</button>
                </div>
              </div>
            </form>
          </div>
        </main>
        <!--TWEEEEEETS-->
        <section id="tweets">
          <!--1 tweet-->
          <div class="tweet-1">
            <div class="tweet-img">
              <img src="/img_avatar.png" alt="Avatar">
            </div>
            <div class="tweet-txt">
              <div class="tweet-name-date">
                <strong> Shloch</strong>
                <span class="twitter-account"> @shloch</span> - <span class="date">Nov 11</span>
              </div>
              <div class="message"> Building the Portfolio page of a graphic designer (Infinity Graphics) </div>
              <div class="tweet-icons">
                <i class="fas fa-image"></i>
                <i class="fas fa-gift"></i>
                <i class="fas fa-signal"></i>
                <i class="fas fa-smile"></i>
              </div>
            </div>
          </div>
        </section>
      </div>
      <!--Right  block-->
      <div class='col-lg-3 d-none d-lg-block' id="rightBlock">
        <!--proposed profiles-->
        <div class="other-profiles">
          <div class="heading">
            <h5>Who to follow</h5>
          </div>
          <div class="profile-1">
            <div class="profile-img">
              <img src="/img_avatar2.png" class="avatar" alt="Avatar">
            </div>
            <div class="profile-name"> CTE Magazine <br />
              <span class="twitter-account">@CTEMagPlus</span>
            </div>
            <div class="follow-btn">
              <button>Follow</button>
            </div>
          </div>
          <div class="profile-1">
            <div class="profile-img">
              <img src="/img_avatar.png" class="avatar" alt="Avatar">
            </div>
            <div class="profile-name"> CTE Magazine <br />
              <span class="twitter-account">@CTEMagPlus</span>
            </div>
            <div class="follow-btn">
              <button>Follow</button>
            </div>
          </div>
          <div class="profile-1">
            <div class="profile-img">
              <img src="/img_avatar2.png" class="avatar" alt="Avatar">
            </div>
            <div class="profile-name"> CTE Magazine <br />
              <span class="twitter-account">@CTEMagPlus</span>
            </div>
            <div class="follow-btn">
              <button>Follow</button>
            </div>
          </div>
          <div class="heading">
            <a href="#">Show more</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>