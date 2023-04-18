# LMN-Chat-Widget
Add voices (input and output) to a web-friendly chatbot widget

The text-only chat widget based on https://github.com/JiteshGaikwad/Chatbot-Widget 
## How to add chatbot to your website

add the following code to your website

```
      <div id="chatbot">initial content</div>
      <script type="text/javascript" src="static/js/chatbot.js"></script>
```

Change the `/static/js/constants.js` to point to different chatbot server. Change the `/static/js/chatbot.js` to modify the chatbot widget behavior.

To launch a local echo chatbot server, run the following command

```
cd api
python chatbot.py
```
## References

I have added the voices to the Chatbot Widget:

- https://github.com/mdn/web-speech-api/tree/master/speak-easy-synthesis
- https://developer.mozilla.org/en-US/docs/Web/API/SpeechSynthesisUtterance/SpeechSynthesisUtterance
- https://mdn.github.io/web-speech-api/speak-easy-synthesis/
- https://www.studytonight.com/post/javascript-speech-recognition-example-speech-to-text

## Hot to get all the voices:
```
if (theVoice == null) {
    let voices = synth.getVoices();
    for(i = 0; i < voices.length ; i++) {
        if(voices[i].name === "Google UK English Male") {
            utterThis.voice = voices[i];
            theVoice = voices[i];
            console.log("Voice is set.");
            break;
        }
    }
}
```

## Get free background
https://unsplash.com/
