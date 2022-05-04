<template>
  <nav>
    <ul>
      <li v-for="title in navMenu" :key="title.id">
        <a href="#">{{ title.name }}</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "NavComponent",
  data() {
    return {
      navMenu: [{
        id:1,
        name:"Characters",
      },
      {
        id:2,
        name:"Comics",
      },
      {
        id:3,
        name:"Movies",
      },
      {
        id:4,
        name:"Tv",
      },
      {
        id:5,
        name:"Games",
      },
      {
        id:6,
        name:"Collectables",
      },
      {
        id:7,
        name:"Videos",
      },
      {
        id:8,
        name: "Fans",
      },
      {
        id:9,
        name:"News",
      },
      {
        id:10,
        name:"Shop",
      }    
      ],
    };
  },
};
</script>

<style lang="scss" scoped>

ul {
  list-style: none;
  display: flex;
  justify-content: center;
  align-content: center;
  li {
    padding: 0 1rem;

    a {
      text-decoration: none;
      text-transform: uppercase;
      font-size: 14px;
      font-weight: 400;
      padding: 2.375rem 0;
      color: black;
    }

    &:hover a {
      color: $primaryColor;
      box-shadow: 0px 8px $primaryColor;
    }
  }
}
</style>