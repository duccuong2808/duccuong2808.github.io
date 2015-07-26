####Setting


```ruby
class test
  def test1
  end
end

```

#####*Preferences.sublime-settings*

```JSON
{
    "Seti_blue_tab_label": true,
    "Seti_no_bar_undertabs": true,
    "Seti_pad_3": true,
    "Seti_rainbow": true,
    "Seti_sb_small_padding": true,
    "Seti_tabs_small": true,
    "always_show_minimap_viewport": true,
    "auto_complete": true,
    "auto_complete_commit_on_tab": true,
    "bold_folder_labels": true,
    "color_scheme": "Packages/User/SublimeLinter/primer.dark (SL).tmTheme",
    "copy_with_empty_selection": true,
    "ensure_newline_at_eof_on_save": true,
    "font_face": "Source Code Pro",
    "font_options":
    [
        "gray_antialias"
    ],
    "font_size": 9,
    "ignored_packages":
    [
        "Vintage"
    ],
    "index_files": true,
    "line_padding_top": 3,
    "material_theme_small_tab": true,
    "overlay_scroll_bars": "enabled",
    "rulers":
    [
        80,
        100,
        120
    ],
    "telex": true,
    "theme": "Primer Dark.sublime-theme",
    "theme_primer_tab_active_green": true,
    "translate_tabs_to_spaces": true,
    "trim_trailing_white_space_on_save": true
}
```

#####*Default (Linux).sublime-keymap*

```JSON
[
  { "keys": ["f12"], "command": "htmlprettify"},
  { "keys": ["f1"], "command": "fold" },
  { "keys": ["f2"], "command": "unfold" },
  { "keys": ["ctrl+l"], "command": "show_overlay", "args": {"overlay": "goto", "text": "@"} },

  { "keys": ["ctrl+space"], "command": "auto_complete" },
  { "keys": ["ctrl+space"], "command": "replace_completion_with_auto_complete", "context":
    [
      { "key": "last_command", "operator": "equal", "operand": "insert_best_completion" },
      { "key": "auto_complete_visible", "operator": "equal", "operand": false },
      { "key": "setting.tab_completion", "operator": "equal", "operand": true }
    ]
  },
  { "keys": ["ctrl+d"], "command": "run_macro_file", "args": {"file": "Packages/Default/Delete Line.sublime-macro"} },
  { "keys": ["ctrl+shift+c"], "command": "toggle_comment", "args": { "block": false } },
  { "keys": ["ctrl+shift+c"], "command": "toggle_comment", "args": { "block": true } },
  { "keys": ["ctrl+shift+f"], "command": "reindent" , "args": {"single_line": false}},
  { "keys": ["alt+up"], "command": "swap_line_up" },
  { "keys": ["alt+down"], "command": "swap_line_down" },
  { "keys": ["ctrl+alt+j"], "command": "join_lines" },
  { "keys": ["ctrl+alt+down"], "command": "duplicate_line" },
  { "keys": ["shift+ctrl+r"], "command": "show_overlay", "args": {"overlay": "goto", "show_files": true} },
  { "keys": ["ctrl+shift+s"], "command": "save_all" },
  { "keys": ["ctrl+l"], "command": "show_overlay", "args": {"overlay": "goto", "text": ":"} },
  { "keys": ["shift+ctrl+f4"], "command": "close_all" },
  { "keys": ["shift+ctrl+y"], "command": "lower_case" },
  { "keys": ["shift+ctrl+x"], "command": "upper_case" }
]
```
