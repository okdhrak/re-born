<template>
  <section class="container">
    <h1>{{title}}</h1>

  </section>
</template>


<script>
export default {
	head: {
		//title: '俺のホームページ 🚀',
	},
	head () {
	    return {
	      script: [
	        { src: 'https://cdnjs.cloudflare.com/ajax/libs/jquery/3.1.1/jquery.min.js' }
	      ],
	      link: [
	        { rel: 'stylesheet', href: 'https://fonts.googleapis.com/css?family=Roboto&display=swap' }
	      ]
	    }
	  },
  data: function(){
    return {
      title:'Hello',
      message: 'this is message.',
    };
  },
};
</script>

<style>
/*@import "../assets/common.css";*/
</style>

<style lang="scss">
body {
	background: #EDEDED;
	a {
		font-size: 30px !important;
		color: red;
		&:hover {
			color: yellow;
		}
	}
}
a {
  font-size:16pt;
}
.link {
  background-color: #def;
  padding:10px;
}
.container {
  padding:5px 10px;
}
h1 {
  font-size: 60pt;
  color: #345980;
}
p {
  padding-top:5px;
  font-size: 20pt;
}
pre {
  padding: 10px;
  font-size: 18pt;
  background-color: #efefef;
}
hr {
  margin:10px 0px;
}
</style>
