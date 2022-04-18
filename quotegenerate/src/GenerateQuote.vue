<template>
    <div class="center">
<h1>Random Quote Generator</h1>
    <p>{{ quote.quote }}</p>
    <p> {{ quote.cite }}</p>
  <button class="btn" @click="generate">New Quote</button>
  </div>
</template>

<script>
const quotes = [
  {
    quote:
      "The purpose of our lives is to be happy.",
    cite: " Dalai Lama",
  },
  {
    quote:
      "Get busy living or get busy dying.",
      cite: "Stephen King"
  },
  {
    quote: "You only live once, but if you do it right, once is enough.",
    cite: " Mae West",
  },
  {
    quote: "Talk is cheap. Show me the code.",
    cite: "Linus Torvalds",
  },
  {
    quote:
      "Always code as if the guy who ends up maintaining your code will be a violent psychopath who knows where you live.",
    cite: "Martin Golding",
  },
  {
    quote:
      "Most good programmers do programming not because they expect to get paid or get adulation by the public, but because it is fun to program.",
    cite: "Linus Torvalds",
  },
  {
    quote:
      "Most software today is very much like an Egyptian pyramid with millions of bricks piled on top of each other, with no structural integrity, but just done by brute force and thousands of slaves.",
    cite: "Alan Kay",
  },
  {
    quote:
      "Most of you are familiar with the virtues of a programmer. There are three, of course: laziness, impatience, and hubris",
    cite: "Larry Wall",
  },
  {
    quote:
      "First learn computer science and all the theory. Next develop a programming style. Then forget all that and just hack.",
    cite: "George Carrette",
  },
  {
      quote: "Many of life’s failures are people who did not realize how close they were to success when they gave up.",
      cite:"Thomas A. Edison"
  },
  {
      quote: "In order to write about life first you must live it.",
      cite: "Ernest Hemingway"
  },
  {
      quote: "My mama always said, life is like a box of chocolates. You never know what you’re gonna get.",
      cite: " Forrest Gump"
  },
  {
      quote: "Every moment is a fresh beginning.",
      cite: "T.S. Eliot"
  }
];

export default {
  name: "App",
  data() {
    return { quote: {} };
  },
  methods: {
    generate() {
      const index = Math.floor(Math.random() * quotes.length);
      this.quote = quotes[index];
    },
  },
}; 

</script>

<style >
.center {
  margin: auto;
  width: 50%;
  border: 5px solid orange;
  padding: 60px;
}
.btn {
  position: absolute;
  top: 65%;
  left: 50%;
  transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  background-color: #f1f1f1;
  color: black;
  font-size: 16px;
  padding: 16px 30px;
  border: none;
  cursor: pointer;
  border-radius: 5px;
  text-align: center;
}

 .btn:hover {
  background-color: rgb(251, 180, 47);
  color: rgb(0, 0, 0);
}
p{
  background-color: orange;
  color: black;
  font-size: 18px;
}
</style>