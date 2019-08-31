<template>
  <div>
		<p>number is {{count}}</p>
		<button @click="inc">+</button>&emsp;&emsp;
		<button @click="dec">-</button>
	</div>
</template>

<script>
	export default {
		data() {
			return {
				count: 0
			}
		},
		methods: {
			//增加
			inc() {
				const count = this.count
				this.count = count + 1
			},
			//减少
			dec() {
        const count = this.count
        if(count > 0){
          this.count = count - 1
        }else{
          this.count = count
        }
				
			}
		},
	}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
