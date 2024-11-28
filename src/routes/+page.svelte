<script>
    // List of random words
    const words = ['Serendipity', 'Cascade', 'Whisper', 'Luminous', 'Echo', 
        'Nebula', 'Zenith', 'Aurora', 'Breeze', 'Crystal', 'Enigma', 
        'Harmony', 'Melody', 'Velvet', 'Dream'];
    
    // Variable to store current word
    let currentWord = 'Click anywhere';
    
    // Function to get random word
    function getRandomWord() {
        const randomIndex = Math.floor(Math.random() * words.length);
        currentWord = words[randomIndex];
    }
</script>

<div on:click={getRandomWord}>
    <h1>{currentWord}</h1>
</div>

<style>
    div {
        height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        cursor: pointer;
    }

    h1 {
        font-size: 3rem;
    }
</style>