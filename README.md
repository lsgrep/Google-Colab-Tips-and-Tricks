# [Google Colab](https://colab.research.google.com/) Tips and Tricks


### Editor
If you are comfortable Vim you can enable Vim keyboard bindings from the settings.

### Shortcuts
Majority of Colab shortcuts are multi step shortcuts like Emacs. For example, 
to see all the available shortcuts you have to press`Command/Ctrl + m` prefix first then press`h`.

It is too much mental burden to remember every single shortcut, 
so typing out the command via command palette(`Command/Ctrl+Shift+p`) is not a bad idea.
![command_palette](https://raw.githubusercontent.com/lsgrep/Google-Colab-Tips-and-Tricks/master/assets/command-palette.png)


### Terminal
Terminal have a builtin Tmux, which is neat for creating multiple panes. 
The downside is though you have to learn the Tmux shortcuts if you are not familiar with it.
As always, there must be a ton of tutorial on YouTube.
 

### Building Colab Desktop App

![desktop_demo](https://raw.githubusercontent.com/lsgrep/Google-Colab-Tips-and-Tricks/master/assets/desktop-app-demo.png)

I was skeptical at first then I am liking the desktop app more than I should. 

The following command can be used to create Colab app on macOS with [nativefier](https://github.com/jiahaog/nativefier).

```shell
nativefier --name "Colab" \
  --internal-urls "(.*?contacts\.google\.com.*?|.*?accounts\.google\.com.*?|.*?colab\.research\.google\.com.*?)" \
  --single-instance --icon assets/Colab.png  https://colab.research.google.com
```

You have to switch the icon file to the corresponding one based on your system.
- `.ico` - For Windows
- `.icns` or `.png` - For macOS (Apple Icon Image format)
- `.png` - For Linux

### More
- [Configuring Google Colab Like A Pro](https://medium.com/@robertbracco1/configuring-google-colab-like-a-pro-d61c253f7573)
