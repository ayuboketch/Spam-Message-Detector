![Screen Shot 2024-02-09 at 18 01 54](https://github.com/ayuboketch/Spam-Message-Detector/assets/17433791/e9bff2d6-eb9e-40bc-b9de-a36b39de005b)
![Screen Shot 2024-02-09 at 18 01 23](https://github.com/ayuboketch/Spam-Message-Detector/assets/17433791/13a7e9d5-625c-4c55-b38b-0f79f872913d)

# Spam-Message-Detector
🚀 Project: Spam Message Detector

In this JavaScript project, I created a simple spam message detector using regular expressions. The application takes user input from a message input field, applies various regex patterns to identify potential spam content, and provides real-time feedback.
# Key Features:

    Regex Patterns: Utilized multiple regular expressions to detect patterns commonly associated with spam, including pleas for help, monetary requests, free offers, stock alerts, and friendly greetings.
    Dynamic Check: The application dynamically checks user input against the predefined regex patterns to determine if the message is likely spam.
    User Feedback: Delivers immediate feedback to the user, indicating whether the entered message appears to be spam or not.
This project showcases the power of regular expressions in identifying specific content patterns, making it a valuable tool for filtering and analyzing text input. Users can now receive quick alerts about potential spam messages, enhancing communication security.

# Sample JavaScript Code:

javascript
// [Code snippet from the project]
const isSpam = (msg) => denyList.some((regex) => regex.test(msg));

checkMessageButton.addEventListener("click", () => {
  if (messageInput.value === "") {
    alert("Please enter a message.");
    return;
  }

  result.textContent = isSpam(messageInput.value)
    ? "Oh no! This looks like a spam message."
    : "This message does not seem to contain any spam.";
  messageInput.value = "";
});
