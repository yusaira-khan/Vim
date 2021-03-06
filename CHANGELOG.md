## 0.2.1

* Normal and visual keys can now be defined in .keymap instead of .behaviors
  * Use :editor.keys.vim.normal.cm tag in keymap instead of deprecated lt.plugins.vim/map-keys behavior
    For example, `[:app :lt.plugins.vim/map-keys {"j" "gj" "k" "gk"}]` in a behaviors file,
    is `[:editor.keys.vim.normal.cm "j" "gj"] [:editor.keys.vim.normal.cm "k" "gk"]` in a keymap file.
  * Use :editor.keys.vim.visual.cm tag in keymap instead of deprecated lt.plugins.vim/map-keys-visual behavior
* Fix normal mode interacting with autoclose-brackets behavior and inserting paired characters
* Add :qa ex command

## 0.2.0

* Plugin activated by default. :lt.plugins.vim/activate-vim behavior in
  user.behaviors no longer needed
* Convert keymap and behaviors to flat format
* Add K as a :editor.doc.toggle binding
* Add :lt.plugins.vim/set-options behavior

## 0.1.0

* Update vim.js to CM 4.6.0 - adds C-v and more
  * See http://codemirror.net/doc/releases.html for more
* Fix macros and display their status with cm.openDialog
* Add tabn and tabp ex-commands
* Remove unused behaviors
