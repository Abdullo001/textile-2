<template >
  <div class="sidebar-wrapper">
    <div class="sitelogo-wrapper">
      <nuxt-link to="/" active-class="active"
        ><SiteLogo class="site-logo"
      /></nuxt-link>
    </div>

    <nav>
      <ul class="nav-list">
        <li class="nav-item">
          <nuxt-link to="/home" class="nav-link">
            <div class="d-flex align-center">
              <img src="~assets/images/dashboard.svg" alt="dashboard" />
              <span>Dashboard</span>
            </div>
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/a" class="nav-link">
            <div>
              <img src="~assets/images/user.svg" alt="user" />
              <span>User</span>
            </div>
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/s" class="nav-link">
            <div>
              <img src="~assets/images/localization.svg" alt="localization" />
              <span>Localization</span>
            </div>
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/d" class="nav-link">
            <div>
              <img src="~assets/images/prefinances.svg" alt="prefinances" />
              <span>Prefinances</span>
            </div>
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/f" class="nav-link">
            <div>
              <img src="~assets/images/fraud.svg" alt="fraud" />
              <span>Fraud management</span>
            </div>
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/g" class="nav-link">
            <div>
              <img src="~assets/images/access.svg" alt="access" />
              <span>Access control</span>
            </div>
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/h" class="nav-link">
            <div>
              <img src="~assets/images/billing.svg" alt="billing" />
              <span>Billing</span>
            </div>
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/lists" class="nav-link">
            <div>
              <img src="~assets/images/lists.svg" alt="lists" />
              <span>Lists</span>
            </div>
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/k" class="nav-link">
            <div>
              <img src="~assets/images/catalogs.svg" alt="catalogs" />
              <span>catalogs</span>
            </div>
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/l" class="nav-link">
            <div>
              <img src="~assets/images/planning.svg" alt="planning" />
              <span>Planning</span>
            </div>
          </nuxt-link>
        </li>
        <li class="nav-item">
          <nuxt-link to="/z" class="nav-link">
            <div>
              <img src="~assets/images/settings.svg" alt="settings" />
              <span>Settings</span>
            </div>
          </nuxt-link>
        </li>
      </ul>
    </nav>
  </div>
</template>
<script>
import SiteLogo from "../assets/images/SiteLogo.vue";
export default {
  components: {
    SiteLogo,
  },
};
</script>
<style scoped lang="scss" >
.sidebar-wrapper {
  width: 296px;
  padding: 24px;
  display: flex;
  flex-direction: column;
  align-items: center;

  background-color: #ffffff;
}

.sitelogo-wrapper {
  margin-bottom: 66px;
}

.nav-list {
  list-style-type: none;
}

.nav-item {
  width: 248px;
  display: flex;
  flex-direction: row;
  align-items: center;
}

.nav-item:last-child {
  margin-bottom: 82px;
}

.nav-link {
  display: block;
  width: 100%;
  padding: 14px 16px;

  font-weight: 500;
  text-decoration: none;
  font-size: 16px;
  line-height: 22px;
  color: #777c85;
  background-color: transparent;
  transition: all ease 0.3s;

  border-radius: 8px;

  div {
    display: flex;
    align-items: center;

    img {
      margin-right: 8px;
    }
  }
}

.nuxt-link-active {
  background: rgba(111, 49, 237, 0.2);

  color: #7631ff;
}
</style>