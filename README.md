!https://s3.amazonaws.com/ohmyzsh/oh-my-zsh-logo.png!

oh-my-zsh is an open source, community-driven framework for managing your ZSH configuration. It comes bundled with a ton of helpful functions, helpers, plugins, themes, and few things that make you shout...

bq. "OH MY ZSHELL!"

h2. Setup

@oh-my-zsh@ should work with any recent release of "zsh":http://www.zsh.org/, the minimum recommended version is 4.3.9.

h3. The automatic installer... (do you trust me?)

You can install this via the command line with either `curl` or `wget`.

h4. via `curl`

@curl -L https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh | sh@

h4. via `wget`

@wget --no-check-certificate https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O - | sh@

h3. The manual way


1. Clone the repository

@git clone git://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh@

2. *OPTIONAL* Backup your existing ~/.zshrc file

@cp ~/.zshrc ~/.zshrc.orig@

3. Create a new zsh config by copying the zsh template we've provided.

@cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc@


4. Set zsh as your default shell:

@chsh -s /bin/zsh@

5. Start / restart zsh (open a new terminal is easy enough...)

h3. Problems?

You _might_ need to modify your PATH in ~/.zshrc if you're not able to find some commands after switching to _Oh My Zsh_.

h2. Usage

* enable the plugins you want in your @~/.zshrc@ (take a look at @plugins/@ to see what's possible)
  ** example: @plugins=(git osx ruby)@
* Theme support: Change the @ZSH_THEME@ environment variable in @~/.zshrc@.
  ** Take a look at the "current themes":https://wiki.github.com/robbyrussell/oh-my-zsh/themes that come bundled with _Oh My Zsh_.
* much much more...  take a look at @lib/@ what _Oh My Zsh_ offers...

h2. Useful

the "refcard":http://www.bash2zsh.com/zsh_refcard/refcard.pdf is pretty tasty for tips.

h3. Customization

If you want to override any of the default behavior, just add a new file (ending in @.zsh@) into the @custom/@ directory.
If you have many functions which go well together you can put them as a *.plugin.zsh file in the @custom/plugins/@ directory and then enable this plugin.
If you would like to override the functionality of a plugin distributed with oh-my-zsh, create a plugin of the same name in the @custom/plugins/@ directory and it will be loaded instead of the one in @plugins/@.

h3. Updates

By default you will be prompted to check for updates. If you would like oh-my-zsh to automatically update itself without prompting you, set the following in your ~/.zshrc

@DISABLE_UPDATE_PROMPT=true@

To disable updates entirely, put this in your ~/.zshrc

@DISABLE_AUTO_UPDATE=true@

To upgrade directly from the command line, just run @upgrade_oh_my_zsh@

h3. Uninstalling

If you want to uninstall it, just run @uninstall_oh_my_zsh@ from the command line and it'll remove itself and revert you to bash (or your previous zsh config).

h2. Help out!

I'm far from being a zsh-expert and suspect there are many ways to improve. If you have ideas on how to make the configuration easier to maintain (and faster), don't hesitate to fork and send pull requests!

h3. (Don't) Send us your theme! (for now)

-I'm hoping to collect a bunch of themes for our command prompts. You can see existing ones in the @themes/@ directory.-

We have enough themes for the time being. Please fork the project and add on in there, you can let people know how to grab it from there.

h2. Contributors

This project wouldn't exist without all of our awesome users and contributors.

* "View our growing list of contributors":https://github.com/robbyrussell/oh-my-zsh/contributors

Thank you so much!
