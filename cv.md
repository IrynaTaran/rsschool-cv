# rsschool-cv
## Iryna Taran
## Contacts
* **Location:** Berlin, Germany
* **Phone:** +49 0152 271 741 34
* **Email:** irayegay659@gmail.com
* **GitHub:** IrynaTaran
* **Telegram:** @io_taran
## About me
I am 23 y.o., from Ukraine. I have a bachelor's degree in marketing. I have 2 years of experience as an administrator in top-3 Ukrainian PR agency "Mainstream". I am currently studying to be a front-end developer.
## Skills
* JavaScript (beginner)
* HTML (beginner)
* CSS (beginner)
## Code example
Task from book "JavaScript for kids" – create a hangman game.

```
<!DOCTYPE html>
<html>
    <head>
        <title>Hangman</title>
    </head>
    <body>
        <h3>Let's play Hangman game</h3>
        <p>Try to guess the word! He-he-he!!!</p>
        <p>Just reload the page to start. Good luck!</p>
        <script>
            var words = [
                "hemisphere",
                "donkey",
                "treasure",
                "wardrobe",
                "parachute",
                "movie",
                "button",
                "picture"
            ]
            var word = words[Math.floor(Math.random() * words.length)];
            var answerArray = [];
            for (var i = 0; i < word.length; i++) {
                answerArray[i] = "_";
            }
            var remainingLetters = word.length;
            var guesses = 20;
            while (remainingLetters > 0 && guesses > 0) {
                alert(answerArray.join(" "));
                var guess = prompt("Enter a letter or click Cancel to exit");
                if (guess === null) {
                    break;
                } else if (guess.length !==1) {
                    alert("Please, enter a single letter");
                } else {
                    guess = guess.toLowerCase();
                    guesses --;
                    for (var j = 0; j < word.length; j++) {
                        if (word[j] === guess && answerArray[j] === "_") {
                            answerArray[j] = guess;
                            remainingLetters--;
                        }
                    }
                }
            }
            alert(answerArray.join(" "));
            if (guesses > 0) {
            alert("Great! The word was: " + word + ".");
            } else {
                alert("You loose, try again! The word was: " + word + ".");
            }
        </script>
    </body>
</html>
```

## Experience
Have no experience yet
## Education
* Kyiv National Economic University, bachelor's degree in marketing
* Courses:
    + CodeCademy JavaScript
    + Code-basics HTML
    + Code-basics CSS
## Languages
* Ukrainian – native
* Russian – fluent
* English – fluent
* German – level B2
