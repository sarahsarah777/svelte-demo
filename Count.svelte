<script>
		import BarGauge from "./BarGauge.svelte";
		import DropGauge from "./DropGauge.svelte";
		let count = 0;

		function handleSubtract() {
		  count -= 10;
		}
		function handleAdd() {
		  count += 10;
		}
</script>

<style>
	.flex-row {
	  display: flex;
	  width: 100%;
	  align-items: center;
	  justify-content: center;
	}
	#count {
	  margin: 20px;
	  font-size: 30px;
	  width: 100px;
	}
	button {
	  background: #ffffff;
	  color: #1f1f1f;
	  border: 1px solid #d4d4d4;
	  padding: 8px 12px;
	  border-radius: 2px;
	  cursor: pointer;
	}
	*:disabled {
	  background-color: #f3f3f3;
	  color: #d4d4d4;
	  opacity: 1;
	  cursor: not-allowed !important;
	}
</style>

<div class='flex-row'>
	<button on:click={handleSubtract} disabled={count == 0}>
		-
	</button>
	<div id='count'>{count}</div>
	<button on:click={handleAdd} disabled={count == 100}>
		+
	</button>
</div>

<br/>

<BarGauge count={count}/>

<br/>

<DropGauge count={count}/>