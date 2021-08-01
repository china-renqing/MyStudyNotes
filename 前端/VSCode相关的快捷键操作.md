# VSCode相关的快捷键操作

* 在Jason文件中加入该代码即可（**设置**→**键盘快捷方式**→**打开键盘快捷键方式(JSON)**右上角）

* ```json
      //上下左右快捷键
      {
          "key": "alt+i",
          "command": "cursorUp",
          "when": "textInputFocus"
      },
      {
          "key": "up",
          "command": "cursorUp",
          "when": "textInputFocus"
      },
      {
          "key": "alt+k",
          "command": "cursorDown",
          "when": "textInputFocus"
      },
      {
          "key": "down",
          "command": "cursorDown",
          "when": "textInputFocus"
      },
      {
          "key": "alt+j",
          "command": "cursorLeft",
          "when": "textInputFocus"
      },
      {
          "key": "left",
          "command": "cursorLeft",
          "when": "textInputFocus"
      },
      {
          "key": "alt+l",
          "command": "cursorRight",
          "when": "textInputFocus"
      },
      {
          "key": "right",
          "command": "cursorRight",
          "when": "textInputFocus"
      },
      {
          "key": "down",
          "command": "list.focusDown",
          "when": "listFocus && !inputFocus"
      },
      {
          "key": "down",
          "command": "selectNextSuggestion",
          "when": "suggestWidgetMultipleSuggestions && suggestWidgetVisible && textInputFocus"
      },
      {
          "key": "alt+k",
          "command": "selectNextSuggestion",
          "when": "suggestWidgetMultipleSuggestions && suggestWidgetVisible && textInputFocus"
      },
      {
          "key": "up",
          "command": "selectPrevSuggestion",
          "when": "suggestWidgetMultipleSuggestions && suggestWidgetVisible && textInputFocus"
      },
      {
          "key": "alt+i",
          "command": "selectPrevSuggestion",
          "when": "suggestWidgetMultipleSuggestions && suggestWidgetVisible && textInputFocus"
      },
  
      //跳转到文本末、文本首的快捷键
      {
          "key": "alt+o",
          "command": "cursorEnd",
          "when": "textInputFocus"
      },
      {
          "key": "end",
          "command": "cursorEnd",
          "when": "textInputFocus"
      },
      {
          "key": "alt+u",
          "command": "cursorHome",
          "when": "textInputFocus"
      },
      {
          "key": "home",
          "command": "cursorHome",
          "when": "textInputFocus"
      },
  
      //跳词快捷键
      {
          "key": "ctrl+alt+j",
          "command": "cursorWordLeft",
          "when": "textInputFocus"
      },
      {
          "key": "ctrl+alt+l",
          "command": "cursorWordRight",
          "when": "textInputFocus"
      }，
  //选中快捷键
      {
          "key":"alt+shift+j",
          "command":"cursorLeftSelect",
          "when": "textInputFocus"
      },
      {
          "key":"alt+shift+l",
          "command":"cursorRightSelect",
          "when": "textInputFocus"
      },
      {
          "key":"alt+shift+i",
          "command":"cursorUpSelect",
          "when": "textInputFocus"
      },
      {
          "key":"alt+shift+k",
          "command":"cursorDownSelect",
          "when": "textInputFocus"
      },
      {
          "key":"ctrl+alt+shift+j",
          "command":"cursorWordLeftSelect",
          "when": "textInputFocus"
      },
      {
          "key":"ctrl+alt+shift+l",
          "command":"cursorWordRightSelect",
          "when": "textInputFocus"
      }
  ```
  
* 参考以下博客和官网

  * [VS code设置双快捷键](https://www.aukocharlie.com/archives/vscode%E8%AE%BE%E7%BD%AE%E5%8F%8C%E5%BF%AB%E6%8D%B7%E9%94%AE)
  * [VS code官网 Key Bidings](https://code.visualstudio.com/docs/getstarted/keybindings)

* 

