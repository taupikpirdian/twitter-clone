<template>
    <div class='col-lg-3 col-md-1 col-2'>
        <nav>
          <a href="#">
            <i class="fab fa-twitter fa-2x"></i>
          </a>
          <ul class="nav flex-column">
            <li class="nav-item">
              <a class="nav-link active" href="#">
                <font-awesome-icon :icon="['fas', 'fa-house-damage']"/>
                <span class="menu-text">Home</span>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <font-awesome-icon :icon="['fab', 'fa-slack-hash']"/>
                <span class="menu-text">Explore</span>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <font-awesome-icon :icon="['fa', 'fa-bell']"/>
                <span class="menu-text">Notifications</span>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <font-awesome-icon :icon="['fa', 'fa-envelope']"/>
                <span class="menu-text">Messages</span>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <font-awesome-icon :icon="['fa', 'fa-bookmark']"/>
                <span class="menu-text">Bookmarks</span>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <font-awesome-icon :icon="['fa', 'fa-list-alt']"/>
                <span class="menu-text">Lists</span>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <font-awesome-icon :icon="['fa', 'fa-user']"/>
                <span class="menu-text">Profile</span>
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <font-awesome-icon :icon="['fas', 'fa-ellipsis-h']" />
                <span class="menu-text">Mores</span>
              </a>
            </li>
            <li class="nav-item mobile-post">
              <a class="nav-link2" href="#">
                <i class="far fa-edit"></i>
              </a>
            </li>
          </ul>
          <button type="button" class="btn btn-primary btn-sm tweeterBtn"> Tweet</button>
        </nav>
    </div>
</template>