# Pi Coding Agent

Pi (version 0.79.3) is installed with npm as a global module from @earendil-works/pi-coding-agent. If you install a new version of Node or npm with e.g. nvm, it may break your pi setup. Then you have to save the models.json file again for Pi to see the configuration again.

The config file includes a configuration for a local coding model. You can install local models from e.g. HuggingFace and load them on your computer with LM Studio. You must load the model that best suits your hardware and then serve the model via a localhost server so it can be loaded with Pi.
