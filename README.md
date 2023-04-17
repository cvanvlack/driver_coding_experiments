# Driver Coding Experiments
This is a description of how I have tried to use AutoGPT

## ChatGPT Example
[Here](https://shareg.pt/qnvHjtb) is me trying to implement the driver using ChatGPT along with GPT4. 

Techniques I used as part of this coversation:
\* When I had multiple sections to copy in, I ended a prompt with 'But wait, I have more info. Just answer with READ:'. This allowed me to copy in more info and then continue the conversation without having to wait for ChatGPT to generate a long response and waste the calculation time with all of those tokens.
\* I had to provide direct links to the manuals.
\* Initially, I just asked it to write a command to read the version number. It didn't respect the formatting at all. I had to redo the prompt and try to describe what the command format was like with reference to specific sections in the manual.

Some examples of things I would like to have seen improved by this code:
\* There's no handling of the response to check for errors from the device.
\* Ideally, we would have responses to things like "Pressure Units" to be mapped to enums for the rest of the application to use.
\* There's no error handling. I would like to see the code handle errors and try to recover from them. Ideally with a difference between recoverable errors (timeouts, device connection issues, etc...) and non-recoverable errors.
\* What happens in the constructor if there's an error connecting to the device?


