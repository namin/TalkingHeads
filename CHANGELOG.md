## 0.5.4 (2024-11-18)

### Fix

- **ChatGPT**: New XPATH for text input

## 0.5.3 (2024-11-05)

### Fix

- Introduced generic tests
- Xpath updates for ChatGPT, Copilot, HuggingChat
- **HuggingChat**: only click close button if it is present, and do not throw error because of the button
- **ChatGPT**: Regenerate function try again button included
- **Copilot**: fix various login issues
- **Copilot**: Skip location modal in case it pops.
- **Copilot**: Remove reduntant imports
- **Copilot**: Reworked prompting, image utility, interact and reset_thread to be compatible with the new Copilot UI
- **Copilot**: Plugin and model features removed.
- **base_browser**: Docstrings, linting and formatting


## 0.5.2 (2024-08-11)

### Fix
- XPATH elements updated for ChatGPT, Gemini, and LeChat
- **gemini**: The response is retrieved repeatedly and is returned once the streaming has finished.
- **lechat**: Fixed the model button click.
- **chatgpt**: Removed unnecessary waiting for send button
- **test**: New model name for LeChat, different order in Gemini, 

## 0.5.1 (2024-06-05)

### Fix
- XPATH elements updated for ChatGPT, Gemini, and HuggingChat
- timeout_dur removed from super class initialization
- **base_browser**: Explicit timeout_dur setting, multihead waiting procedure
- **chatgpt**: Removed unnecessary waiting for send button
- **huggingface**: Model switch modal closes if fails
- **gemini**: Clicks the data privacy "Got it" button if pops up
- **multiagent**: Instead of launching browsers concurrently, launch them one after another, in sequence.

## 0.5.0 (2024-03-18)

### Features

- **is_url_check_filetype**: new functions to check filetype and if the string is url
- **lechat**: Mistral Le Chat is automated
- **gemini_multimodal**: It is possible to upload image to Gemini
- **image**: Implementation of image upload feature
- **multiagent**: First commit of Multiagent subpackage including Conversation
- **reset_thread**: now it is possible to reset chat, disabled model switch

### Fix

- **import**: Changed init file
- **logging**: import logging removed
- **object_markers**: Fixed old markers and new file format
- **init**: Initialization fixes
- **logging_and_driver_arguments**: It is now possible to pass driver arguments as dictionary
- **logging_interacting**: Logging changed to instance based logger and fixed a bug in interaction
- **claude**: Fixed a response error
- **logging**: uses it's own logging
