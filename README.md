[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/NUTiSmoa)
 Ced-Man: Your Friendly Cybersecurity Chatbot

[ **Ced-Man** is a simple, console-based cybersecurity awareness chatbot built in C#. It's designed to provide basic information and tips on common cybersecurity topics like passwords, scams, privacy, and phishing. Ced-Man can also remember your name and your favorite cybersecurity topic for a more personalized interaction.

## Features

* **Keyword Recognition:** Understands basic cybersecurity terms and provides relevant information.
* **Flexible Tip Responses:** Offers a variety of tips for topics like scams, phishing, and passwords.
* **Sentiment Detection:** Attempts to recognize basic user sentiment (worried, curious, frustrated, confused, unsure) and responds appropriately.
* **Memory and Recall:** Remembers your name and preferred cybersecurity topic.
* **Conversation Flow:** Can provide more details on the last discussed topic when asked.
* **ASCII Art Logo:** Features a friendly "Ced-Man" logo on startup.
* **(Optional) Voice Greeting:** Plays an audio greeting (if the `recording-audio.wav` file is found at the specified path).

## Getting Started

### Prerequisites

* [.NET SDK](https://dotnet.microsoft.com/download) installed on your system.
* (Optional) A `.wav` audio file named `recording-audio.wav` located at `C:\Users\Cedri\OneDrive\Documents\chat10bot\ConsoleApp1\bin\Debug\` for the voice greeting to work. You can remove or modify this functionality in the code if you don't have this file or prefer not to use it.

### Running the Chatbot

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/ST10348711/.git](https://github.com/ST10348711.git)
    
    ```
    

2.  **Navigate to the Project Directory:**
    ```bash
    cd ChatbotV1
    ```
    (Or the directory containing the `.csproj` file)

3.  **Run the Chatbot:**
    ```bash
    dotnet run
    ```

    This command will build and execute the chatbot in your console.

4.  **Interact with Ced-Man:** Type your cybersecurity-related questions or statements and press Enter.

5.  **Exit the Chatbot:** Type `exit` and press Enter to close the application.

## How to Use

Here are some examples of how you can interact with Ced-Man:

* `Tell me about passwords.`
* `What are some scam tips?`
* `I'm worried about phishing.`
* `My name is Alice.`
* `I'm interested in network security.`
* `What's my name?`
* `What am I interested in?`
* `Explain further.` (after a previous response)
* `More details on privacy.`

## Code Structure

The main logic of the chatbot is contained within the `Program.cs` file:

* `PlayVoiceGreeting()`: (Optional) Plays an audio greeting.
* `DisplayAsciiLogo()`: Displays the "Ced-Man" ASCII art.
* `userName`: Stores the user's name.
* `favouriteCybersecurityTopic`: Stores the user's preferred topic.
* `KeywordResponses`: A dictionary mapping keywords to direct responses.
* `FlexibleResponses`: A dictionary mapping arrays of keywords to random tip responses.
* `SentimentResponses`: A dictionary mapping sentiment keywords to appropriate responses.
* `GetResponse(string userInput)`: The core method that processes user input and generates a response.
* `ContainsAll(string input, IEnumerable<string> keywords)`: Helper function to check if all keywords are present in the input.
* `GetRandomElement(string[] array)`: Helper function to get a random element from an array.
* `ProvideMoreDetails(string topic)`: Provides follow-up information on a given topic.
* `Main(string[] args)`: The entry point of the application, handling the main interaction loop.

## Contributing

Contributions to Ced-Man are welcome! If you have ideas for new features, improved responses, or bug fixes, feel free to:

1.  Fork the repository.
2.  Create a new branch for your changes (`git checkout -b feature/your-feature-name`).
3.  Make your changes and commit them (`git commit -am 'Add some feature'`).
4.  Push to the branch (`git push origin feature/your-feature-name`).
5.  Open a pull request.

## License

This project is licensed under the [MIT License](LICENSE). See the `LICENSE` file for more details.

## Acknowledgements

* Inspired by the need for basic cybersecurity awareness.
* Utilizes the .NET SDK for development.

---

**Stay safe online! - Ced-Man**
