<script>
    let url = '';

    function shortenUrl() {
        console.log(url);
    }
</script>

<div>
    <input type="text" placeholder="Insert your URL" bind:value={url}>
    <button on:click={shortenUrl}>Shorten</button>
</div>

<style>
    div {
        background-color: var(--dark);
        padding: 1rem;
        color: #fff;
        display: flex;
        flex-direction: column;
        gap: 1rem;
    }

    input {
        border-radius: 10px;
        border: none;
        padding: 1rem;
        font-size: 1.1rem;
    }

    button {
        padding: 1rem;
        background-color: var(--amazon);
        color: #fff;
        border: none;
        border-radius: 10px;
        font-size: 1.1rem;
        cursor: pointer;
        transition: all .1s linear;
    }

    button:hover {
        background-color: var(--mint);
    }

    @media screen and (min-width: 1000px) {
        div {
            align-items: center;
            justify-content: space-evenly;
            flex-direction: row;
            padding: 1rem 10rem;
        }
        input {
            width: 100%;
        }
        button {
            width: 20%;
        }
    }
</style>