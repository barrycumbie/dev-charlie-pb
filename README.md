# Whack-a-Monster

A simple browser game where players click monsters to earn points before time runs out!

## Authorship

- **Author:** Parker Bell
- **GitHub:** [pbell0330](https://github.com/pbell0330)
- **Project:** dev|charlie
- **Version:** 1.0
- **Date:** 2026-10-13

## User Story

- **As a** visitor to my GitHub profile,
- **I want** to play a quick monster-clicking game,
- **So that** I can have fun and try to beat my high score.

## Narrative

Whack-a-Monster is a simple browser-based arcade game. Players start a round and click monsters to earn points. The goal is to score as many points as possible before the 30-second timer reaches zero. Players can enter a name or play as a guest.

## About the App

### Planning and Game Ideas

- **Planning issue:** [Whack-a-Monster Game Ideas and Planning](https://github.com/pbell0330/dev-charlie/issues/new)
- **Wiki:** [View the project Wiki](https://github.com/pbell0330/dev-charlie/wiki)

Replace the three placeholder URLs above with your actual GitHub links.

### Directory Structure

```text
dev-charlie/
├── index.html
├── README.md
├── wireframe.png
```

### Technologies and Tools

- HTML5 for page structure
- CSS3 for styling
- JavaScript for game logic
- jQuery for click events and page updates
- Bootstrap 5 for layout and components
- Bootstrap Icons for the navigation icon
- Bootstrap modal for the leaderboard
- sessionStorage for temporary leaderboard scores
- GitHub for version control, issues, Wiki, and Pages
- Visual Studio Code for editing code

### How the Game Works

1. The player enters a name or plays as a guest.
2. The player clicks Start Game.
3. Clicking the monster earns 10 points.
4. The timer counts down from 30 seconds.
5. When time runs out, the final score is displayed.
6. Scores are saved temporarily in the browser session.

### Code Example

The following JavaScript handles monster clicks and increases the score:

```javascript
holes.on("click", function () {
  if (playing && holes.index(this) === monster) {
    score += 10;
    $("#score").text(score);
    showMonster();
  }
});
```

This event checks whether the game is running and whether the player clicked the current monster. If both conditions are true, it increases the score and displays another monster.

### Validation and Accessibility

- Used buttons for interactive game spaces and controls.
- Added labels for the player name input.
- Used an accessible live region for game messages.
- Used readable text and contrasting colors.
- Tested starting, resetting, scoring, and ending a game.
- Further accessibility and browser testing can be completed as improvements.


### Sprint 99: Future Ideas

- Add new difficulty levels.
- Add sound effects.
- Add more monsters and bonus points.

See the Sprint 99 milestone and related issues in the repository.

## Links

- **Play the game:** [https://pbell0330.github.io/dev-charlie/](https://pbell0330.github.io/dev-charlie/)
- **Repository:** [https://github.com/pbell0330/dev-charlie](https://github.com/pbell0330/dev-charlie)
- **GitHub Profile:** [https://github.com/pbell0330](https://github.com/pbell0330)

