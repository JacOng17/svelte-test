<script>
	let count = 0;
	$: doubled = count * 2;
	$: if (count >= 100) {
		alert(`count is dangerously high!`);
		count = 9;
	}
	
	function handleClick() {
		count += 1;
	}
</script>

<button on:click={handleClick}>
	Clicked {count} {count === 1 ? 'time' : 'times'}
</button>
<p>{count} doubled is {doubled}</p>
