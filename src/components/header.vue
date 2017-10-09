<template lang="html">
  <header>
	  <div class="logo">
	  	Open Politics
	  </div>
	  <ul>
		  <li v-for="listmenu in listmenus">
			  {{ listmenu.message }}
		  </li>
	  </ul>
  </header>
</template>

<script>
export default {
	name: 'header',
	data () {
return {     listmenus: [
	       { message: 'Home' },
	       { message: 'Profile' },
	       { message: 'Settings' },
	       { message: 'Sign Out' }
     		]
		}
	}
}
</script>

<style lang="scss">
	header{
		width: 100%;
		height: 200px;
		background-color: brown;
	}
</style>
