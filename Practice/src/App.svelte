<script>


let firstname ='Mahesh';
let lastname = 'Mandale';
let beltColour ='Orange';

	$: fullname = {firstname} ,{lastname}
	$: console.log (beltColour)


	const handleClick=()=>{
		beltColour='Black';
	};

	const handleInput=(e) => {
		beltColour= e.target.value
	};

</script>

<main>
	
	<p>{fullname} - {beltColour} belt</p>
	
	<!-- <button on:click={handleClick}>Update BeltColour</button> -->
	<!-- <input type="text" on:input={handleInput} value={beltColour}> -->
	<input type="text" bind:value={firstname}>
	<input type="text" bind:value={lastname}>
	<input type="text" bind:value={beltColour}>
</main>

<style>
main{
	text-align: center;
}
</style>
