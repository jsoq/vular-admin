<template>
  <div id="app">
    <VularAdmin />
  </div>
</template>

<script>
  export default {
    name: 'app',
    data: () => ({
      admins: [
      ['Management', 'people_outline'],
      ['Settings', 'settings'],
      ],
      cruds: [
      ['Create', 'add'],
      ['Read', 'insert_drive_file'],
      ['Update', 'update'],
      ['Delete', 'delete'],
      ],
      drawers: ['Default (no property)', 'Permanent', 'Temporary'],
      primaryDrawer: {
        model: null,
        type: 'default (no property)',
        clipped: false,
        floating: false,
        mini: false,
      },
      footer: {
        inset: false,
      },

      adminApp:{
        fontFamily:"",
        logo: {
          src: "images/logo.png",
          title:"Vular",
          alt: "An amazing framework",
        },
        drawer: {
          showLogo: true,
          color: "#1b1b28",
          logoColor: "#1a1a27",
          textColor:"",
          activeTextColor:"",
          subheaderColor:"",
          fontSize:"0.825rem",
          dark:true,
          logoDark:true,
        },
        appbar:{
          showLogo:false,
          dark:true,
        },
      }
    }),
  }
</script>

<style>
#app {
}

/*::-webkit-scrollbar {
  width: 0.3rem;
  height: 0.3rem;
}
::-webkit-scrollbar-track {
  border-radius: 0;
}
::-webkit-scrollbar-thumb {
  border-radius: 0;
  background: #535353;
  transition: all .2s;
}
::-webkit-scrollbar-thumb:hover {
  background-color: #606060;
}

::-webkit-scrollbar-corner{
  background: #232323;
  }*/
  body{
    font-size:13px;
  }

  h1, h2 {
    font-weight: normal;
  }

  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }

  a {
    color: #42b983;
  }
</style>
