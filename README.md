# My emacs configuration

To get started clone the repository and add the following to your `.emacs` file:

```
(require 'package)
(setq package-enable-at-startup nil)
(add-to-list 'package-archives
             '("melpa" . "https://melpa.org/packages/"))
(package-initialize)

;; Bootstrap 'use-package'
(unless (package-installed-p 'use-package)
  (package-refresh-contents)
  (package-install 'use-package))

(org-babel-load-file (expand-file-name "<path to my_init.org>"))
```

**Change `"<path to my_init.org>"` to the path to the `my_init.org` file in the cloned repository.**