<p align="center">
  <img width="800" src="./screenshot.png">
</p>

# What is sort-tab?
sort-tab is smarter tab solution for Emacs, it sort tab with using frequency.

sort-tab stay on top of Emacs, it won't waste any vertically space when you split window.

## Installation
1. Clone or download this repository (path of the folder is the `<path-to-sort-tab>` used below).
2. In your `~/.emacs`, add the following two lines:
```elisp
(add-to-list 'load-path "<path-to-sort-tab>") ; add sort-tab to your load-path
(require 'sort-tab)
(sort-tab-mode 1)
```

## Usage
* sort-tab-select-next-tab: select next tab
* sort-tab-select-prev-tab: select previous tab
* sort-tab-select-first-tab: select first tab
* sort-tab-select-last-tab: select last tab
* sort-tab-close-current-tab: close current tab

#### SwitchTabByIndex
You can bind the number keys to the command ```sort-tab-select-visible-tab```, such as s-1, s-2, s-3 ... etc.

```
(global-set-key (kbd "s-1") 'sort-tab-select-visible-tab)
(global-set-key (kbd "s-2") 'sort-tab-select-visible-tab)
(global-set-key (kbd "s-3") 'sort-tab-select-visible-tab)
(global-set-key (kbd "s-4") 'sort-tab-select-visible-tab)
(global-set-key (kbd "s-5") 'sort-tab-select-visible-tab)
(global-set-key (kbd "s-6") 'sort-tab-select-visible-tab)
(global-set-key (kbd "s-7") 'sort-tab-select-visible-tab)
(global-set-key (kbd "s-8") 'sort-tab-select-visible-tab)
(global-set-key (kbd "s-9") 'sort-tab-select-visible-tab)
(global-set-key (kbd "s-0") 'sort-tab-select-visible-tab)
(global-set-key (kbd "s-Q") 'sort-tab-close-all-tabs)
```

This function automatically recognizes the number at the end of the keystroke
and switches to the tab of the corresponding index.
