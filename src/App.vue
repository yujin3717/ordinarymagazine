<template>
	<div id="wrap" class="max-container">
		<Spinner v-show="loading"/>
		<!-- <Cover/> -->
		<!-- <Guide/> -->
		<Header/>
		<Drawer/>
		<Main @setSpinner="setSpin"/>
		<Footer/>
	</div>
</template>

<script>
import Main from '@/components/main/Main.vue'
import Header from '@/components/header/Header.vue'
import Cover from '@/components/cover/Cover.vue'
import Guide from '@/components/guide/Guide.vue'
import Drawer from '@/components/navigation/Drawer.vue'
import Footer from '@/components/footer/Footer.vue'
import Spinner from '@/components/spinner/Spinner.vue'

export default {
	components:{
		Main,
		Header,
		Cover,
		Guide,
		Drawer,
		Footer,
		Spinner
	},
	data(){
		return{
			loading: true
		}
	},
	mounted(){

	},
	methods:{
		setSpin: function() {
			var self = this;
			console.log("setSpinner");
			this.$nextTick(function() {
				setTimeout(() => {
					self.loading = !self.loading;
				}, 1000);
			});
		}
	}
}
</script>

<style lang="scss">

</style>
