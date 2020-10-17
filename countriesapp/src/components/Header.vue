<template>
  <header id="header">
    <div class="topnav">
      <a class="active" href="#home">Home</a>
      <a href="#news">Where In The World?</a>
      <div class="topnav-right">
        <button @click="toggleViewModel">Dark Mode</button>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      darkMode: false,

      countries: {
        id: "USA",
        name: "United States of America",
      },
    };
  },
  methods: {
    toggleViewModel() {
      console.log("DARK MODE SEQUENCE INITIATED");
      this.darkMode = !this.darkMode;
    },
  },
};
</script>

<style>


/* Style the links inside the navigation bar */
.topnav{
  font-family: 'Nunito Sans', sans-serif;
  font-weight: 800; 

}
.topnav a {
  
  float: left;
  color:black;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 20px;
}

/* Change the color of links on hover */
.topnav a:hover {
  color: black;
}

/* Add a color to the active/current link */
.topnav a.active {
color:black
}

/* Right-aligned section inside the top navigation */
.topnav-right {
  float: right;
}
</style>