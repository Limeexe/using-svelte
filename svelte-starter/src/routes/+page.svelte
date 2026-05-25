<script>
    let count = $state(0);

    let doubleCount = $derived(count *2);

    $effect(()=>{
        console.log(`Count: ${count}, Double Count: ${doubleCount}`);
    });

    function increment(){
        count++;
    }

    function reset(){
        count = 0;
    }
</script>

<button onclick={increment}>Increment</button>
<button onclick={reset}> Reset</button>

<h1>Count: {count} <br> Double Count: {doubleCount}</h1>