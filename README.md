```md
# Bot Battlr

Bot Battlr is a React application that allows users to browse through a list of robots, view their details, and enlist or release them into/from their bot army. This application was built as a code challenge to demonstrate proficiency in React concepts such as props, events, rendering, and code structure/efficiency.

## Features

### Bot Collection
- Displays a list of all available bots, each with its name, avatar, and basic stats (health, damage, armor, and bot class).

### Bot Details
- Clicking on a bot in the collection reveals more detailed information about the bot, including its catchphrase and creation/update timestamps.

### Enlist Bot
- Users can enlist an individual bot into their army by clicking on it in the collection.
- The selected bot will be rendered in the "Your Bot Army" section.

### Release Bot
- Users can release a bot from their army by clicking on it in the "Your Bot Army" section.
- The bot will be removed from the army but remain in the overall collection.

### Discharge Bot
- Users can permanently discharge a bot from service by clicking the red "x" button next to the bot in the "Your Bot Army" section.
- This will delete the bot from both the backend server and the frontend.

## Technologies Used

- React.js
- JSON Server
- Fetch API

## Getting Started

To run the Bot Battlr application locally, follow these steps:

### Clone the Repository

```
git clone https://github.com/Nyandiekahh/Code-Challenge-Bot-Battlr
```

### Install Dependencies

```
cd bot-battlr
npm install
```

### Start the JSON Server

```
json-server --watch db.json
```

This will start the local server at `http://localhost:8001/`.

### Start the React Development Server

In a separate terminal window, run the following command:

```
npm start
```

This will open the application in your default browser at `http://localhost:3000/`.

## Code Structure

The main components of the Bot Battlr application are:

### App.js
- The root component that holds the state for bot data and the user's army.

### BotCollection.js
- Renders a list of all available bots from the server.

### YourBotArmy.js
- Displays the bots that the user has enlisted into their army.

The application follows a unidirectional data flow, where the `App.js` component serves as the single source of truth for bot data and the user's army. Data is passed down to child components as props, and events (such as enlisting or releasing a bot) are handled by callback functions passed down from the parent component.

## Contributing

Contributions to the Bot Battlr application are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

When contributing, please follow the existing code style and conventions, and make sure to include tests for any new functionality or bug fixes.

### Submitting Issues

1. Go to the repository's Issues tab.
2. Click the "New Issue" button.
3. Provide a clear and descriptive title for the issue.
4. In the issue body, describe the problem or suggestion in detail.
5. If applicable, include steps to reproduce the issue.
6. Click "Submit new issue" to create the issue.

### Submitting Pull Requests

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make the necessary changes and commit them.
4. Push your changes to your forked repository.
5. Go to the original repository and click the "New Pull Request" button.
6. Select your forked repository and branch.
7. Provide a clear and descriptive title for the pull request.
8. In the pull request body, describe the changes you've made.
9. Click "Create Pull Request" to submit your changes for review.

## License

This project is licensed under the [MIT License](LICENSE).
```
