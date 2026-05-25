<script>
    let count = $state(0);

    let doubleCount = $derived(count *2);

    function reset(){
        count = 0;
    }
</script>

<button onclick={()=>count++}>Increment</button>
<button onclick={reset}> Reset</button>

<h1>Count: {count} <br> Double Count: {doubleCount}</h1>