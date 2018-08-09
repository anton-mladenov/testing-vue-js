<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
	<h3>{{ msg2 }}</h3>
	<h6> {{ msg3 }} </h6>
	<div>
		<h4> 
			{{ msg4 }}
		</h4>
	</div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
	  	let msg = 'Anton says Hi'
		let msg4 = msg.length > 4 ? "Hey Anton is here!" : "Where is Anton?"
		return {
		msg,
		msg2: "some real Vue JS testing is going on around here",
		msg3: "hahahah just kidding!",
		msg4
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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
