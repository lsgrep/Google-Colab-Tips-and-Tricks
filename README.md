# Google Colab Tips and Tricks


### Editor
If you are comfortable VIM you can enable VIM bindings from the settings.

### Shortcuts
Majority of Colab shortcuts are multi step shortcuts. For example, 
to see all the available shortcuts you have to press`Command/Ctrl and M` first then press`h`  


### Terminal
Terminal have a builtin Tmux, which is neat for creating multiple panes.
 

### Build Colab Desktop App
I was skeptical at first then I am liking the desktop app more than I should. 

The following command can be used to create Colab app on macOS.

```shell
nativefier --name "Colab" \
  --internal-urls "(.*?contacts\.google\.com.*?|.*?accounts\.google\.com.*?|.*?colab\.research\.google\.com.*?)" \
  --single-instance --icon ../Colab.png  https://colab.research.google.com
```

You have to switch the icon to the corresponding one based on your system.
- `.ico` - For Windows
- `.icns` or `.png` - For macOS (Apple Icon Image format)
- `.png` - For Linux


