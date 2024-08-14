
<template>
  <div class="banner">
    <video autoplay muted loop class="banner-video">
      <source src="../../assets/media/banner.mp4" type="video/mp4" />
    </video>
    <div class="banner-content">
      <v-container fluid>
        <v-row align="center">
          <v-col cols="12" md="9">
            <v-row align="center">
              <v-col cols="12" sm="4" md="3" lg="2">Duong Jerry</v-col>
              <v-col cols="12" sm="4" md="3" lg="2">
                <v-speed-dial
                  location="bottom bottom"
                  transition="slide-x-transition"
                >
                  <template v-slot:activator="{ props: activatorProps }">
                    <v-fab v-bind="activatorProps" size="small" variant="text"
                      >ELECTRIC
                      <v-icon class="ml-4" icon="$expand"></v-icon>
                    </v-fab>
                  </template>
                  <div class="menu-right-one"></div>
                  <v-btn key="1" icon="$success"></v-btn>
                  <v-btn key="2" icon="$info"></v-btn>
                  <v-btn key="3" icon="$warning"></v-btn>
                  <v-btn key="4" icon="$error"></v-btn>
                </v-speed-dial>
              </v-col>
              <v-col cols="12" sm="4" md="3" lg="2">
                <v-speed-dial
                  location="bottom bottom"
                  transition="slide-x-transition"
                >
                  <template v-slot:activator="{ props: activatorProps }">
                    <v-fab v-bind="activatorProps" size="small" variant="text"
                      >ELECTRIC
                      <v-icon class="ml-4" icon="$expand"></v-icon>
                    </v-fab>
                  </template>
                  <div class="menu-right-tow"></div>
                  <v-btn key="1" icon="$success"></v-btn>
                  <v-btn key="2" icon="$info"></v-btn>
                  <v-btn key="3" icon="$warning"></v-btn>
                  <v-btn key="4" icon="$error"></v-btn>
                </v-speed-dial>
              </v-col>
              <v-col cols="12" sm="4" md="3" lg="2">
                <v-speed-dial
                  location="bottom bottom"
                  transition="slide-x-transition"
                >
                  <template v-slot:activator="{ props: activatorProps }">
                    <v-fab v-bind="activatorProps" size="small" variant="text"
                      >ELECTRIC
                      <v-icon class="ml-4" icon="$expand"></v-icon>
                    </v-fab>
                  </template>
                  <div class="menu-right-three"></div>
                  <v-btn key="1" icon="$success"></v-btn>
                  <v-btn key="2" icon="$info"></v-btn>
                  <v-btn key="3" icon="$warning"></v-btn>
                  <v-btn key="4" icon="$error"></v-btn>
                </v-speed-dial>
              </v-col>
            </v-row>
          </v-col>
          <v-col cols="12" md="3">
            <v-row align="center">
              <v-col>
                <v-icon icon="mdi mdi-user"></v-icon>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { text: "Real-Time", icon: "mdi-clock" },
        { text: "Audience", icon: "mdi-account" },
        { text: "Conversions", icon: "mdi-flag" },
      ],
    };
  },
  props: {
    title: {
      type: String,
      default: "Welcome to Our Website",
    },
    subtitle: {
      type: String,
      default: "Your subtitle goes here",
    },
  },
};
</script>

<style scoped>
.banner {
  position: relative;
  width: 100%;
  height: 100vh;
  overflow: hidden;
}
.menu-right-one {
  margin: 5vh 0px 0px 0px;
}
.menu-right-tow {
  margin: 25vh 0px 0px 0px;
}
.menu-right-three {
  margin: 45vh 0px 0px 0px;
}
.banner-video {
  position: absolute;
  top: 50%;
  left: 50%;
  min-width: 100%;
  min-height: 100%;
  width: auto;
  height: auto;
  transform: translate(-50%, -50%);
  z-index: 1;
  object-fit: cover;
}

.banner-content {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 2;
  color: white;
  background: rgba(0, 0, 0, 0.25);
}


.banner h1 {
  font-size: 3rem;
  margin: 0;
}

.banner p {
  font-size: 1.5rem;
}
</style>
