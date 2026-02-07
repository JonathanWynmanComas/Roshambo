let wins = 0;
let losses = 0;
let ties = 0;

const choices = ["R", "P", "S"];

function playGame() {
    let userChoice = prompt("Enter R for Rock, P for Paper, or S for Scissors").toUpperCase();

    if (!choices.includes(userChoice)) {
        alert("Invalid choice. Please enter R, P, or S.");
        return;
    }

    let computerChoice = choices[Math.floor(Math.random() * choices.length)];

    let result = "";

    if (userChoice === computerChoice) {
        ties++;
        result = "It's a tie!";
    } else if (
        (userChoice === "R" && computerChoice === "S") ||
        (userChoice === "P" && computerChoice === "R") ||
        (userChoice === "S" && computerChoice === "P")
    ) {
        wins++;
        result = "You win!";
    } else {
        losses++;
        result = "You lose!";
    }

    alert(
        "You chose: " + userChoice +
        "\nComputer chose: " + computerChoice +
        "\n\n" + result +
        "\n\nWins: " + wins +
        "\nLosses: " + losses +
        "\nTies: " + ties
    );
}

do {
    playGame();
} while (confirm("Do you want to play again?"));
