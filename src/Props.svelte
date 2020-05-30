<script>
    export let hoge = 'default value.'
	export let answer = 'default value.';
    export let price;
    export let amount;

    $:total = price * amount;
</script>

<p>The answer is {answer}</p>
<p>This is {hoge}</p>
<p>Total is {total}</p>
