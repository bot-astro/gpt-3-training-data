# GPT-3 training data
This repository holds the `training.jsonl` file.  
This file contains a set of question & answers that are used to train a chatGPT model.  

This way it's possible to train chatGPT to respond to questions regarding Astro, helping users understand and use the bot without the need to wait for human support.

## Contribute
To contributo simply fork this repository, add your set of questions and answers and then make a pull request.
### Format of training file
The file `training.jsonl` has a json object for each line.  
Each json object **MUST** have the following form:
```json
{ "prompt": "<question>\n\n===\n\n", "completion": " <answer> END" }
```
It's very important to keep the `\n\n===\n\n` and the **spaces** between the `<answer>`.  

#### Example
```json
{ "prompt": "What is Astro?\n\n===\n\n", "completion": " Astro is a Discord bot that can create temporary voice channels and assign temporary roles to users inside voice channels END" }
```
