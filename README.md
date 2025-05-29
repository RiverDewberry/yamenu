# yamenu
yamenu (Yet Another Menu) is a configurable menu that only shows entries listed in its config file. It is designed to be used as an application launcher with yamenu-run 
# Dependencies
 - python 3.13+
 - raylib 5.5+
# Configuration
yamenu searches for the config file in the folowing location: ~/.config/yamenu/config.json if you wish to change this
The following elements in the config file are used by yamenu:
 - "entries": an array of arrays of strings which represent the entries in the menu, the first element in each array in "entries" is the term that can be searched for in the menu, the last element in each array is the output of the menu if that entry is selected, and the second element, if there is a second element, is displayed next to the search term as a description. An ecample of an element in "entries" is ["mc", "minecraft", "minecraft-launcher"]. This would be displayed as "mc (minecraft)" and would output "minecraft-launcher" if selected. If there is a second element, but that secend element is "", then no description is shown, for ecample ["mc", "", "minecraft-launcher"] would be displayed as only "mc"
 - "font": the path to a .ttf file used as the font for the menu. startmenu.ttf is not set as the default in the config file, however it is provided to be used with yamenu although any .ttf should work
 - "colors": an object containing elements that control what color each part of yamenu is. The valid colors are as follows: "darkgray", "maroon", "orange", "darkgreen", "darkblue", "darkpurple", "darkbrown", "gray", "red", "gold", "lime", "blue", "violet", "brown", "lightgray", "pink", "yellow", "green", "skyblue", "purple", "beige", "white", and "black"
 - "font_size": the size of the font
 - "letter_spacing": extra spacing between letters
 - "cmd_spacing": the spacing between each entry in the menu
 - "screen_width": the width of the window created by the menu
 - "screen_height": the height of the window created by the menu
 - "left_gap": the gap between the left side of the window and the left side of the menu
 - "top_gap": the gap between the top of the window and the top of the menu
 - "right_gap": the gap between the right side of the window and the right side of the menu
 - "bottom_gap": the gap between the bottom of the window and the bottom of the menu
 - "left_border": the size of the border on the left 
 - "top_border": the size of the border on the top
 - "right_border": the size of the border on the right
 - "bottom_border": the size of the border on the bottom
 - "bar_top_gap": the gap between the bottom of the input and the top of the bar
 - "bar_height": the height of the bar
 - "bar_bottom_gap": the gap between the bottom of the bar and the entries
 - "dot_size": the size of the dot
 - "dot_gap_left": the gap between the left of the window and the dot
 - "dot_gap_top": the gap between the y pos of the selected entry ond the dot
 - "input_offset": the gap between the left side of the window and the input
 - "command_offset": the gap between the left side of the screen and the entries
 - "no_input_text": text shown when no input is entered
 - "max_input_len": maximum length of the input
 - "cursor_on_time": the amount of time the cursor is on
 - "cursor_off_time": the amount of time the cursor is off
# Installation
make a config file at ~/.config/yamenu/config.json or move config.json to that location
